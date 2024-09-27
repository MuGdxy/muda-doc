

# File buffer\_info\_accessor.h

[**File List**](files.md) **>** [**buffer**](dir_9b44f68c181db0b11e9502e462454d05.md) **>** [**buffer\_info\_accessor.h**](buffer__info__accessor_8h.md)

[Go to the documentation of this file](buffer__info__accessor_8h.md)


```C++
#pragma once
#include <utility>
namespace muda::details::buffer
{
class BufferInfoAccessor
{
  public:
    template <typename BufferView>
    static auto cuda_pitched_ptr(BufferView&& b)
    {
        return std::forward<BufferView>(b).cuda_pitched_ptr();
    }
};
}  // namespace muda::details::buffer
```


