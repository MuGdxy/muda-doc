

# File fuzzy.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**fuzzy.h**](fuzzy_8h.md)

[Go to the documentation of this file](fuzzy_8h.md)


```C++
#pragma once
#include <cuda.h>
#include <cuda_runtime.h>
#include <cuda_runtime_api.h>
#include <muda/muda_def.h>

namespace muda
{
template <typename FHost, typename FDevice>
MUDA_INLINE MUDA_GENERIC decltype(auto) invoke(FHost&& host, FDevice&& device) MUDA_NOEXCEPT
{
    if constexpr(std::is_same_v<std::invoke_result_t<FHost>, void>
                 && std::is_same_v<std::invoke_result_t<FDevice>, void>)
    {
#ifdef __CUDA_ARCH__
        device();
#else
        host();
#endif
    }
    else
    {
#ifdef __CUDA_ARCH__
        return device();
#else
        return host();
#endif
    }
}

MUDA_INLINE MUDA_GENERIC dim3 grid_dim()
{
#ifdef __CUDA_ARCH__
    return gridDim;
#else
    return dim3(0, 0, 0);
#endif
}

MUDA_INLINE MUDA_GENERIC dim3 block_idx()
{
#ifdef __CUDA_ARCH__
    return blockIdx;
#else
    return dim3(0, 0, 0);
#endif
}

MUDA_INLINE MUDA_GENERIC dim3 block_dim()
{
#ifdef __CUDA_ARCH__
    return blockDim;
#else
    return dim3(0, 0, 0);
#endif
}

MUDA_INLINE MUDA_GENERIC dim3 thread_idx()
{
#ifdef __CUDA_ARCH__
    return threadIdx;
#else
    return dim3(0, 0, 0);
#endif
}
}  // namespace muda
```


