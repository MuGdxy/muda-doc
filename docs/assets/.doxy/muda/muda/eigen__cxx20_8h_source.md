

# File eigen\_cxx20.h

[**File List**](files.md) **>** [**eigen**](dir_373cdbe7548ceaaa1c4b365fecb08d35.md) **>** [**eigen\_cxx20.h**](eigen__cxx20_8h.md)

[Go to the documentation of this file](eigen__cxx20_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#ifdef __CUDA_ARCH__
#include <complex>
// Fix eigen cuda cxx20 : can't find `arg` in global scope
template <typename T>
MUDA_INLINE MUDA_GENERIC T arg(const std::complex<T>& z)
{
    return std::atan2(std::imag(z), std::real(z));
}
#endif
```


