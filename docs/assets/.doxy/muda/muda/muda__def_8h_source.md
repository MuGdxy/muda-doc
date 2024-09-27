

# File muda\_def.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**muda\_def.h**](muda__def_8h.md)

[Go to the documentation of this file](muda__def_8h.md)


```C++
#pragma once
#include <muda/muda_config.h>
#include <muda/tools/platform.h>
#include <cuda.h>
#include <cuda_runtime.h>
#include <cuda_runtime_api.h>

#define MUDA_HOST __host__
#define MUDA_DEVICE __device__
#define MUDA_GLOBAL __global__
#define MUDA_CONSTANT __constant__
#define MUDA_SHARED __shared__
#define MUDA_MANAGED __managed__

#ifdef __CUDA_ARCH__
#define MUDA_GENERIC MUDA_HOST MUDA_DEVICE
#else
#define MUDA_GENERIC
#endif

// Attributes
#define MUDA_NODISCARD [[nodiscard]]
#define MUDA_DEPRECATED [[deprecated]]
#define MUDA_FALLTHROUGH [[fallthrough]]
#define MUDA_MAYBE_UNUSED [[maybe_unused]]
#define MUDA_NORETURN [[noreturn]]

// Keywords
#define MUDA_NOEXCEPT noexcept
#define MUDA_INLINE inline
#define MUDA_CONSTEXPR constexpr

// Concepts
#if MUDA_HAS_CXX20
#define MUDA_REQUIRES(...) requires (__VA_ARGS__)
#else
#define MUDA_REQUIRES(...)
#endif
```


