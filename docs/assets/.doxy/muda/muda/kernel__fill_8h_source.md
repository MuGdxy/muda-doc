

# File kernel\_fill.h

[**File List**](files.md) **>** [**agent**](dir_b105d52dbe330929a6f21338e69b1ba4.md) **>** [**kernel\_fill.h**](kernel__fill_8h.md)

[Go to the documentation of this file](kernel__fill_8h.md)


```C++
#pragma once
#include <cuda.h>
#include <muda/buffer/buffer_fwd.h>

namespace muda::details::buffer
{
// fill 0D
template <typename T>
MUDA_HOST void kernel_fill(cudaStream_t stream, VarView<T> dst, const T& val);

// fill 1D
template <typename T>
MUDA_HOST void kernel_fill(
    int grid_dim, int block_dim, cudaStream_t stream, BufferView<T> dst, const T& val);

// fill 2D
template <typename T>
MUDA_HOST void kernel_fill(int             grid_dim,
                           int             block_dim,
                           cudaStream_t    stream,
                           Buffer2DView<T> dst,
                           const T&        val);

// fill 3D
template <typename T>
MUDA_HOST void kernel_fill(int             grid_dim,
                           int             block_dim,
                           cudaStream_t    stream,
                           Buffer3DView<T> dst,
                           const T&        val);
}  // namespace muda::details::buffer

#include "details/kernel_fill.inl"
```


