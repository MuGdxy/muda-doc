

# File kernel\_copy\_construct.h

[**File List**](files.md) **>** [**agent**](dir_b105d52dbe330929a6f21338e69b1ba4.md) **>** [**kernel\_copy\_construct.h**](kernel__copy__construct_8h.md)

[Go to the documentation of this file](kernel__copy__construct_8h.md)


```C++
#pragma once
#include <cuda.h>
#include <muda/buffer/buffer_fwd.h>

namespace muda::details::buffer
{
// copy construct 0D
template <typename T>
MUDA_HOST void kernel_copy_construct(cudaStream_t stream,
                                                 VarView<T>   dst,
                                                 CVarView<T>  src);

// copy construct 1D
template <typename T>
MUDA_HOST void kernel_copy_construct(int            grid_dim,
                                                 int            block_dim,
                                                 cudaStream_t   stream,
                                                 BufferView<T>  dst,
                                                 CBufferView<T> src);

// copy construct 2D
template <typename T>
MUDA_HOST void kernel_copy_construct(int              grid_dim,
                                                 int              block_dim,
                                                 cudaStream_t     stream,
                                                 Buffer2DView<T>  dst,
                                                 CBuffer2DView<T> src);

// copy construct 3D
template <typename T>
MUDA_HOST void kernel_copy_construct(int              grid_dim,
                                                 int              block_dim,
                                                 cudaStream_t     stream,
                                                 Buffer3DView<T>  dst,
                                                 CBuffer3DView<T> src);
}  // namespace muda::details::buffer

#include "details/kernel_copy_construct.inl"
```


