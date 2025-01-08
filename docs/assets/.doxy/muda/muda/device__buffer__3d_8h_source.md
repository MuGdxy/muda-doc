

# File device\_buffer\_3d.h

[**File List**](files.md) **>** [**buffer**](dir_9b44f68c181db0b11e9502e462454d05.md) **>** [**device\_buffer\_3d.h**](device__buffer__3d_8h.md)

[Go to the documentation of this file](device__buffer__3d_8h.md)


```C++
/*****************************************************************/

#pragma once
#include <cuda.h>
#include <cuda_runtime.h>
#include <cuda_runtime_api.h>
#include <vector>
#include <muda/viewer/dense.h>
#include <muda/buffer/buffer_3d_view.h>

namespace muda
{
template <typename T>
class DeviceBuffer3D
{
  private:
    friend class BufferLaunch;
    friend class NDReshaper;

    T*       m_data             = nullptr;
    size_t   m_pitch_bytes      = 0;
    size_t   m_pitch_bytes_area = 0;
    Extent3D m_extent           = Extent3D::Zero();
    Extent3D m_capacity         = Extent3D::Zero();

  public:
    using value_type = T;

    DeviceBuffer3D(const Extent3D& n);
    DeviceBuffer3D();

    DeviceBuffer3D(const DeviceBuffer3D<T>& other);
    DeviceBuffer3D(DeviceBuffer3D&& other) MUDA_NOEXCEPT;
    DeviceBuffer3D& operator=(const DeviceBuffer3D<T>& other);
    DeviceBuffer3D& operator=(DeviceBuffer3D<T>&& other);

    DeviceBuffer3D(CBuffer3DView<T> other);
    DeviceBuffer3D& operator=(CBuffer3DView<T> other);

    void copy_to(std::vector<T>& host) const;
    void copy_from(const std::vector<T>& host);

    void resize(Extent3D new_size);
    void resize(Extent3D new_size, const T& value);
    void reserve(Extent3D new_capacity);
    void clear();
    void shrink_to_fit();
    void fill(const T& v);

    Dense3D<T>  viewer() MUDA_NOEXCEPT { return view().viewer(); }
    CDense3D<T> cviewer() const MUDA_NOEXCEPT { return view().viewer(); }

    Buffer3DView<T> view(Offset3D offset, Extent3D extent = {}) MUDA_NOEXCEPT
    {
        return view().subview(offset, extent);
    }
    Buffer3DView<T> view() MUDA_NOEXCEPT
    {
        return Buffer3DView<T>{
            m_data, m_pitch_bytes, m_pitch_bytes_area, Offset3D::Zero(), m_extent};
    }
    operator Buffer3DView<T>() MUDA_NOEXCEPT { return view(); }

    CBuffer3DView<T> view(Offset3D offset, Extent3D extent = {}) const MUDA_NOEXCEPT
    {
        return view().subview(offset, extent);
    }

    CBuffer3DView<T> view() const MUDA_NOEXCEPT
    {
        return CBuffer3DView<T>{
            m_data, m_pitch_bytes, m_pitch_bytes_area, Offset3D::Zero(), m_extent};
    }
    operator CBuffer3DView<T>() const MUDA_NOEXCEPT { return view(); }

    ~DeviceBuffer3D();

    auto extent() const MUDA_NOEXCEPT { return m_extent; }
    auto capacity() const MUDA_NOEXCEPT { return m_capacity; }
    auto pitch_bytes() const MUDA_NOEXCEPT { return m_pitch_bytes; }
    auto pitch_bytes_area() const MUDA_NOEXCEPT { return m_pitch_bytes_area; }
    auto total_size() const MUDA_NOEXCEPT
    {
        return m_extent.width() * m_extent.height() * m_extent.depth();
    }
    T*       data() MUDA_NOEXCEPT { return m_data; }
    const T* data() const MUDA_NOEXCEPT { return m_data; }
};
}  // namespace muda

#include "details/device_buffer_3d.inl"
```


