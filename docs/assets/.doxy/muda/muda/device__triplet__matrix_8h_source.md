

# File device\_triplet\_matrix.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**device\_triplet\_matrix.h**](device__triplet__matrix_8h.md)

[Go to the documentation of this file](device__triplet__matrix_8h.md)


```C++
#pragma once
#include <muda/buffer/device_buffer.h>
#include <muda/ext/linear_system/triplet_matrix_view.h>

namespace muda::details
{
template <typename T, int N>
class MatrixFormatConverter;
}

namespace muda
{
template <typename T, int N>
class DeviceTripletMatrix
{
  public:
    template <typename U, int M>
    friend class details::MatrixFormatConverter;

    using ValueT = std::conditional_t<N == 1, T, Eigen::Matrix<T, N, N>>;
    static constexpr bool IsBlockMatrix = (N > 1);

  protected:
    DeviceBuffer<ValueT> m_values;
    DeviceBuffer<int>    m_row_indices;
    DeviceBuffer<int>    m_col_indices;

    int m_rows = 0;
    int m_cols = 0;

  public:
    DeviceTripletMatrix()                                      = default;
    ~DeviceTripletMatrix()                                     = default;
    DeviceTripletMatrix(const DeviceTripletMatrix&)            = default;
    DeviceTripletMatrix(DeviceTripletMatrix&&)                 = default;
    DeviceTripletMatrix& operator=(const DeviceTripletMatrix&) = default;
    DeviceTripletMatrix& operator=(DeviceTripletMatrix&&)      = default;

    void reshape(int row, int col)
    {
        m_rows = row;
        m_cols = col;
    }

    void resize_triplets(size_t nonzero_count)
    {
        m_values.resize(nonzero_count);
        m_row_indices.resize(nonzero_count);
        m_col_indices.resize(nonzero_count);
    }

    void reserve_triplets(size_t nonzero_count)
    {
        m_values.reserve(nonzero_count);
        m_row_indices.reserve(nonzero_count);
        m_col_indices.reserve(nonzero_count);
    }

    void resize(int row, int col, size_t nonzero_count)
    {
        reshape(row, col);
        resize_triplets(nonzero_count);
    }

    static constexpr int block_dim() { return N; }

    auto values() { return m_values.view(); }
    auto values() const { return m_values.view(); }
    auto row_indices() { return m_row_indices.view(); }
    auto row_indices() const { return m_row_indices.view(); }
    auto col_indices() { return m_col_indices.view(); }
    auto col_indices() const { return m_col_indices.view(); }

    auto rows() const { return m_rows; }
    auto cols() const { return m_cols; }
    auto triplet_count() const { return m_values.size(); }
    auto triplet_capacity() const { return m_values.capacity(); }

    auto view()
    {
        return TripletMatrixView<T, N>{m_rows,
                                       m_cols,
                                       (int)m_values.size(),
                                       m_row_indices.data(),
                                       m_col_indices.data(),
                                       m_values.data()};
    }

    auto view() const { return remove_const(*this).view().as_const(); }

    auto cview() const { return view(); }

    auto viewer() { return view().viewer(); }

    auto cviewer() const { return view().cviewer(); }

    operator TripletMatrixView<T, N>() { return view(); }
    operator CTripletMatrixView<T, N>() const { return view(); }

    void clear()
    {
        m_rows = 0;
        m_cols = 0;
        m_values.clear();
        m_row_indices.clear();
        m_col_indices.clear();
    }
};
}  // namespace muda
#include "details/device_triplet_matrix.inl"
```


