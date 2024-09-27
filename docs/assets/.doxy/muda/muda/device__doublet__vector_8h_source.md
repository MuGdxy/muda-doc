

# File device\_doublet\_vector.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**device\_doublet\_vector.h**](device__doublet__vector_8h.md)

[Go to the documentation of this file](device__doublet__vector_8h.md)


```C++
#pragma once
#include <muda/buffer/device_buffer.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>
#include <muda/ext/linear_system/doublet_vector_view.h>

namespace muda::details
{
template <typename T, int N>
class MatrixFormatConverter;
}

namespace muda
{
template <typename T, int N>
class DeviceDoubletVector
{
    template <typename U, int M>
    friend class details::MatrixFormatConverter;

  public:
    using SegmentVector = Eigen::Vector<T, N>;

  protected:
    muda::DeviceBuffer<SegmentVector> m_segment_values;
    muda::DeviceBuffer<int>           m_segment_indices;
    int                               m_segment_count = 0;

  public:
    DeviceDoubletVector()  = default;
    ~DeviceDoubletVector() = default;

    void reshape(int num_segment) { m_segment_count = num_segment; }

    void resize_doublets(size_t nonzero_count)
    {
        m_segment_values.resize(nonzero_count);
        m_segment_indices.resize(nonzero_count);
    }

    void reserve_doublets(size_t nonzero_count)
    {
        m_segment_values.reserve(nonzero_count);
        m_segment_indices.reserve(nonzero_count);
    }

    void resize(int num_segment, size_t nonzero_count)
    {
        reshape(num_segment);
        resize_doublets(nonzero_count);
    }

    void clear()
    {
        m_segment_values.clear();
        m_segment_indices.clear();
    }

    auto segment_count() const { return m_segment_count; }
    auto segment_values() { return m_segment_values.view(); }
    auto segment_values() const { return m_segment_values.view(); }
    auto segment_indices() { return m_segment_indices.view(); }
    auto segment_indices() const { return m_segment_indices.view(); }

    auto doublet_count() const { return m_segment_values.size(); }
    auto doublet_capacity() const { return m_segment_values.capacity(); }

    auto view()
    {
        return DoubletVectorView<T, N>{m_segment_count,
                                       (int)m_segment_values.size(),
                                       m_segment_indices.data(),
                                       m_segment_values.data()};
    }

    auto view() const { return remove_const(*this).view().as_const(); }

    auto viewer() { return view().viewer(); }
    auto viewer() const { return view().cviewer(); };
};

template <typename T>
class DeviceDoubletVector<T, 1>
{
    template <typename U, int M>
    friend class details::MatrixFormatConverter;

  protected:
    muda::DeviceBuffer<T>   m_values;
    muda::DeviceBuffer<int> m_indices;
    int                     m_size = 0;

  public:
    DeviceDoubletVector()  = default;
    ~DeviceDoubletVector() = default;

    void reshape(int num) { m_size = num; }

    void resize_doublet(size_t nonzero_count)
    {
        m_values.resize(nonzero_count);
        m_indices.resize(nonzero_count);
    }

    void resize(int num, size_t nonzero_count)
    {
        reshape(num);
        resize_doublet(nonzero_count);
    }

    void clear()
    {
        m_values.clear();
        m_indices.clear();
    }

    auto size() const { return m_size; }
    auto values() { return m_values.view(); }
    auto values() const { return m_values.view(); }
    auto indices() { return m_indices.view(); }
    auto indices() const { return m_indices.view(); }
    auto doublet_count() const { return m_values.size(); }

    auto view()
    {
        return DoubletVectorView<T, 1>{
            m_size, (int)m_values.size(), m_indices.data(), m_values.data()};
    }

    auto view() const { return remove_const(*this).view().as_const(); }
    auto viewer() { return view().viewer(); }
    auto viewer() const { return view().cviewer(); };
};
}  // namespace muda

#include "details/device_doublet_vector.inl"
```


