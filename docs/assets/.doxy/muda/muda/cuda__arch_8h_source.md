

# File cuda\_arch.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**type\_traits**](dir_604bea9d06d02462c18f7966e507987c.md) **>** [**cuda\_arch.h**](cuda__arch_8h.md)

[Go to the documentation of this file](cuda__arch_8h.md)


```C++
#pragma once
#include <cuda.h>
namespace muda
{
struct is_cuda_arch
{
#ifdef __CUDA_ARCH__
    constexpr static bool value = true;
#else
    constexpr static bool value = false;
#endif
};

constexpr bool is_cuda_arch_v = is_cuda_arch::value;
}  // namespace muda
```


