

# File atomic.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**atomic.h**](atomic_8h.md)

[Go to the documentation of this file](atomic_8h.md)


```C++
#pragma once
#include <device_atomic_functions.h>
namespace muda
{
template <typename T>
__forceinline__ __device__ T atomic_cas(T* address, T compare, T val)
{
    return atomicCAS(address, compare, val);
}

template <typename T>
__forceinline__ __device__ T atomic_add(T* address, T val)
{
    return atomicAdd(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_sub(T* address, T val)
{
    return atomicSub(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_exch(T* address, T val)
{
    return atomicExch(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_max(T* address, T val)
{
    return atomicMax(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_min(T* address, T val)
{
    return atomicMin(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_and(T* address, T val)
{
    return atomicAnd(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_or(T* address, T val)
{
    return atomicOr(address, val);
}

template <typename T>
__forceinline__ __device__ T atomic_xor(T* address, T val)
{
    return atomicXor(address, val);
}
}  // namespace muda
```


