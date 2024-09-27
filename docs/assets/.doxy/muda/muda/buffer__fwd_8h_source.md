

# File buffer\_fwd.h

[**File List**](files.md) **>** [**buffer**](dir_9b44f68c181db0b11e9502e462454d05.md) **>** [**buffer\_fwd.h**](buffer__fwd_8h.md)

[Go to the documentation of this file](buffer__fwd_8h.md)


```C++
#pragma once

namespace muda
{
template <bool IsConst, typename T>
class VarViewT;

template <typename T>
using VarView = VarViewT<false, T>;

template <typename T>
using CVarView = VarViewT<true, T>;


template <bool IsConst, typename T>
class BufferViewT;

template <typename T>
using BufferView = BufferViewT<false, T>;

template <typename T>
using CBufferView = BufferViewT<true, T>;


template <bool IsConst, typename T>
class Buffer2DViewT;

template <typename T>
using Buffer2DView = Buffer2DViewT<false, T>;

template <typename T>
using CBuffer2DView = Buffer2DViewT<true, T>;


template <bool IsConst, typename T>
class Buffer3DViewT;

template <typename T>
using Buffer3DView = Buffer3DViewT<false, T>;

template <typename T>
using CBuffer3DView = Buffer3DViewT<true, T>;


template <typename T>
class DeviceVar;

template <typename T>
class DeviceBuffer;

template <typename T>
class DeviceBuffer2D;

template <typename T>
class DeviceBuffer3D;
}  // namespace muda
```


