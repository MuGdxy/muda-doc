

# File kernel\_assign.h

[**File List**](files.md) **>** [**agent**](dir_b105d52dbe330929a6f21338e69b1ba4.md) **>** [**kernel\_assign.h**](kernel__assign_8h.md)

[Go to the documentation of this file](kernel__assign_8h.md)


```C++
#pragma once
#include <cuda.h>
#include <muda/buffer/buffer_fwd.h>

namespace muda::details::buffer
{
// assign 0D
template <typename T>
MUDA_HOST void kernel_assign(cudaStream_t stream, VarView<T> dst, CVarView<T> src);

// assign 1D
template <typename T>
MUDA_HOST void kernel_assign(int            grid_dim,
                             int            block_dim,
                             cudaStream_t   stream,
                             BufferView<T>  dst,
                             CBufferView<T> src);

// assign 2D
template <typename T>
MUDA_HOST void kernel_assign(int              grid_dim,
                             int              block_dim,
                             cudaStream_t     stream,
                             Buffer2DView<T>  dst,
                             CBuffer2DView<T> src);

// assign 3D
template <typename T>
MUDA_HOST void kernel_assign(int              grid_dim,
                             int              block_dim,
                             cudaStream_t     stream,
                             Buffer3DView<T>  dst,
                             CBuffer3DView<T> src);
}  // namespace muda::details::buffer

#include "details/kernel_assign.inl"
```


