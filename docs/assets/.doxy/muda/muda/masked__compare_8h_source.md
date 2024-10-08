

# File masked\_compare.h

[**File List**](files.md) **>** [**buffer**](dir_9b44f68c181db0b11e9502e462454d05.md) **>** [**reshape\_nd**](dir_a8e1d5e93e8295fded484e7c98517cd5.md) **>** [**masked\_compare.h**](masked__compare_8h.md)

[Go to the documentation of this file](masked__compare_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <array>
#include <bitset>
namespace muda::details::buffer
{
MUDA_INLINE bool less(bool b, size_t l, size_t r) MUDA_NOEXCEPT
{
    return b ? l < r : true;
}

template <size_t N>
MUDA_INLINE bool less(std::bitset<N>               mask,
                      const std::array<size_t, N>& lhs,
                      const std::array<size_t, N>& rhs) MUDA_NOEXCEPT
{
#pragma unroll
    for(size_t i = 0; i < N; ++i)
        if(!less(mask[i], lhs[i], rhs[i]))
            return false;
    return true;
}
}  // namespace muda::details::buffer
```


