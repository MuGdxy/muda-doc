

# File matrix\_format\_converter\_impl.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**matrix\_format\_converter\_impl.h**](matrix__format__converter__impl_8h.md)

[Go to the documentation of this file](matrix__format__converter__impl_8h.md)


```C++
#pragma once
#include <muda/ext/linear_system/linear_system_handles.h>
#include <muda/ext/linear_system/device_dense_matrix.h>
#include <muda/ext/linear_system/device_dense_vector.h>
#include <muda/ext/linear_system/device_triplet_matrix.h>
#include <muda/ext/linear_system/device_doublet_vector.h>
#include <muda/ext/linear_system/device_bcoo_matrix.h>
#include <muda/ext/linear_system/device_bcoo_vector.h>
#include <muda/ext/linear_system/device_bsr_matrix.h>
#include <muda/ext/linear_system/device_csr_matrix.h>
#include <muda/type_traits/cuda_arch.h>
#include <muda/buffer/device_var.h>

namespace muda
{
namespace details
{
    class MatrixFormatConverterBase
    {
      protected:
        LinearSystemHandles& m_handles;
        cudaDataType_t       m_data_type;
        int                  m_N;

      public:
        MatrixFormatConverterBase(LinearSystemHandles& context, cudaDataType_t data_type, int N)
            : m_handles(context)
            , m_data_type(data_type)
            , m_N(N)
        {
        }

        virtual ~MatrixFormatConverterBase() = default;

        auto dim() const { return m_N; }
        auto data_type() const { return m_data_type; }
        auto cublas() const { return m_handles.cublas(); }
        auto cusparse() const { return m_handles.cusparse(); }
        auto cusolver_sp() const { return m_handles.cusolver_sp(); }
        auto cusolver_dn() const { return m_handles.cusolver_dn(); }

        template <typename T>
        void loose_resize(DeviceBuffer<T>& buf, size_t new_size)
        {
            if(buf.capacity() < new_size)
                buf.reserve(new_size * m_handles.reserve_ratio());
            buf.resize(new_size);
        }
    };

    template <typename T, int N>
    class MatrixFormatConverter : public MatrixFormatConverterBase
    {
        using BlockMatrix   = typename DeviceTripletMatrix<T, N>::BlockMatrix;
        using SegmentVector = typename DeviceDoubletVector<T, N>::SegmentVector;

        DeviceBuffer<int> sort_index;
        DeviceBuffer<int> sort_index_input;
        DeviceBuffer<int> sort_index_tmp;

        DeviceBuffer<int> col_tmp;
        DeviceBuffer<int> row_tmp;

        DeviceBCOOMatrix<T, N> temp_bcoo_matrix;
        DeviceBCOOVector<T, N> temp_bcoo_vector;

        DeviceBuffer<int> unique_indices;
        DeviceBuffer<int> unique_counts;
        DeviceBuffer<int> offsets;

        DeviceVar<int> count;

        DeviceBuffer<int2>     ij_pairs;
        DeviceBuffer<uint64_t> ij_hash;
        DeviceBuffer<uint64_t> ij_hash_input;
        DeviceBuffer<int2>     unique_ij_pairs;

        muda::DeviceBuffer<BlockMatrix> blocks_sorted;
        DeviceBuffer<BlockMatrix>       unique_blocks;
        DeviceBuffer<SegmentVector>     unique_segments;
        DeviceBuffer<SegmentVector>     temp_segments;

        DeviceBuffer<T> unique_values;

      public:
        MatrixFormatConverter(LinearSystemHandles& handles)
            : MatrixFormatConverterBase(handles, cuda_data_type<T>(), N)
        {
        }

        virtual ~MatrixFormatConverter() = default;


        // Triplet -> BCOO
        void convert(const DeviceTripletMatrix<T, N>& from, DeviceBCOOMatrix<T, N>& to);

        void radix_sort_indices_and_blocks(const DeviceTripletMatrix<T, N>& from,
                                           DeviceBCOOMatrix<T, N>& to);
        void make_unique_indices_and_blocks(const DeviceTripletMatrix<T, N>& from,
                                            DeviceBCOOMatrix<T, N>& to);

        void merge_sort_indices_and_blocks(const DeviceTripletMatrix<T, N>& from,
                                           DeviceBCOOMatrix<T, N>& to);
        void make_unique_indices(const DeviceTripletMatrix<T, N>& from,
                                 DeviceBCOOMatrix<T, N>&          to);
        void make_unique_blocks(const DeviceTripletMatrix<T, N>& from,
                                DeviceBCOOMatrix<T, N>&          to);


        // BCOO -> Dense Matrix
        void convert(const DeviceBCOOMatrix<T, N>& from,
                     DeviceDenseMatrix<T>&         to,
                     bool                          clear_dense_matrix = true);

        // BCOO -> COO
        void convert(const DeviceBCOOMatrix<T, N>& from, DeviceCOOMatrix<T>& to);
        void expand_blocks(const DeviceBCOOMatrix<T, N>& from, DeviceCOOMatrix<T>& to);
        void sort_indices_and_values(const DeviceBCOOMatrix<T, N>& from,
                                     DeviceCOOMatrix<T>&           to);

        // BCOO -> BSR
        void convert(const DeviceBCOOMatrix<T, N>& from, DeviceBSRMatrix<T, N>& to);
        void convert(DeviceBCOOMatrix<T, N>&& from, DeviceBSRMatrix<T, N>& to);
        void calculate_block_offsets(const DeviceBCOOMatrix<T, N>& from,
                                     DeviceBSRMatrix<T, N>&        to);

        // Doublet -> BCOO
        void convert(const DeviceDoubletVector<T, N>& from, DeviceBCOOVector<T, N>& to);

        void merge_sort_indices_and_segments(const DeviceDoubletVector<T, N>& from,
                                             DeviceBCOOVector<T, N>& to);
        void make_unique_indices(const DeviceDoubletVector<T, N>& from,
                                 DeviceBCOOVector<T, N>&          to);
        void make_unique_segments(const DeviceDoubletVector<T, N>& from,
                                  DeviceBCOOVector<T, N>&          to);

        // BCOO -> Dense Vector
        void convert(const DeviceBCOOVector<T, N>& from,
                     DeviceDenseVector<T>&         to,
                     bool                          clear_dense_vector = true);
        void set_unique_segments_to_dense_vector(const DeviceBCOOVector<T, N>& from,
                                                 DeviceDenseVector<T>& to,
                                                 bool clear_dense_vector);

        // Triplet -> Dense Vector
        void convert(const DeviceDoubletVector<T, N>& from,
                     DeviceDenseVector<T>&            to,
                     bool clear_dense_vector = true);

        // BSR -> CSR
        void convert(const DeviceBSRMatrix<T, N>& from, DeviceCSRMatrix<T>& to);
    };

    template <typename T>
    class MatrixFormatConverter<T, 1> : public MatrixFormatConverterBase
    {
        DeviceBuffer<int> sort_index;
        DeviceBuffer<int> sort_index_input;
        DeviceBuffer<int> sort_index_tmp;

        DeviceBuffer<int> col_tmp;
        DeviceBuffer<int> row_tmp;

        DeviceBuffer<int>  unique_indices;
        DeviceCOOMatrix<T> temp_coo_matrix;
        DeviceCOOVector<T> temp_coo_vector;

        DeviceBuffer<int> unique_counts;
        DeviceBuffer<int> offsets;

        DeviceVar<int> count;

        DeviceBuffer<int2>     ij_pairs;
        DeviceBuffer<uint64_t> ij_hash;
        DeviceBuffer<uint64_t> ij_hash_input;
        DeviceBuffer<int2>     unique_ij_pairs;

        muda::DeviceBuffer<T> values_sorted;
        DeviceBuffer<T>       unique_values;
        DeviceBuffer<T>       temp_values;

      public:
        MatrixFormatConverter(LinearSystemHandles& handles)
            : MatrixFormatConverterBase(handles, cuda_data_type<T>(), 1)
        {
        }

        virtual ~MatrixFormatConverter() = default;

        // Triplet -> COO
        void convert(const DeviceTripletMatrix<T, 1>& from, DeviceCOOMatrix<T>& to);

        void radix_sort_indices_and_blocks(const DeviceTripletMatrix<T, 1>& from,
                                           DeviceBCOOMatrix<T, 1>& to);
        void make_unique_indices_and_blocks(const DeviceTripletMatrix<T, 1>& from,
                                            DeviceBCOOMatrix<T, 1>& to);

        void merge_sort_indices_and_values(const DeviceTripletMatrix<T, 1>& from,
                                           DeviceCOOMatrix<T>& to);
        void make_unique_indices(const DeviceTripletMatrix<T, 1>& from,
                                 DeviceCOOMatrix<T>&              to);
        void make_unique_values(const DeviceTripletMatrix<T, 1>& from,
                                DeviceCOOMatrix<T>&              to);


        // COO -> Dense Matrix
        void convert(const DeviceCOOMatrix<T>& from,
                     DeviceDenseMatrix<T>&     to,
                     bool                      clear_dense_matrix = true);

        // COO -> CSR
        void convert(const DeviceCOOMatrix<T>& from, DeviceCSRMatrix<T>& to);
        void convert(DeviceCOOMatrix<T>&& from, DeviceCSRMatrix<T>& to);
        void calculate_block_offsets(const DeviceCOOMatrix<T>& from,
                                     DeviceCSRMatrix<T>&       to);

        // Doublet -> COO
        void convert(const DeviceDoubletVector<T, 1>& from, DeviceCOOVector<T>& to);
        void merge_sort_indices_and_values(const DeviceDoubletVector<T, 1>& from,
                                           DeviceCOOVector<T>& to);
        void make_unique_indices(const DeviceDoubletVector<T, 1>& from,
                                 DeviceCOOVector<T>&              to);
        void make_unique_values(const DeviceDoubletVector<T, 1>& from,
                                DeviceCOOVector<T>&              to);


        // COO -> Dense Vector
        void convert(const DeviceCOOVector<T>& from,
                     DeviceDenseVector<T>&     to,
                     bool                      clear_dense_vector = true);
        void set_unique_values_to_dense_vector(const DeviceDoubletVector<T, 1>& from,
                                               DeviceDenseVector<T>& to,
                                               bool clear_dense_vector);

        // Triplet -> Dense Vector
        void convert(const DeviceDoubletVector<T, 1>& from,
                     DeviceDenseVector<T>&            to,
                     bool clear_dense_vector = true);
    };
}  // namespace details
}  // namespace muda

#include "details/matrix_format_converter_impl_block.inl"
#include "details/matrix_format_converter_impl.inl"
```


