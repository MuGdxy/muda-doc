

# File assert.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**assert.h**](assert_8h.md)

[Go to the documentation of this file](assert_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/tools/debug_break.h>

namespace muda
{
MUDA_INLINE MUDA_GENERIC void trap() MUDA_NOEXCEPT
{
#ifdef __CUDA_ARCH__
    __trap();
#else
    std::abort();
#endif
}

MUDA_INLINE MUDA_GENERIC void brkpt() MUDA_NOEXCEPT
{
#ifdef __CUDA_ARCH__
    __brkpt();
#else
    debug_break();
#endif
}
}  // namespace muda
```


