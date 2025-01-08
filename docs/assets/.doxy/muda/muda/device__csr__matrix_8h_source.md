

# File device\_csr\_matrix.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**device\_csr\_matrix.h**](device__csr__matrix_8h.md)

[Go to the documentation of this file](device__csr__matrix_8h.md)


```C++
#pragma once
#include <muda/buffer/device_buffer.h>
#include <muda/ext/linear_system/device_bsr_matrix.h>
#include <cusparse.h>
#include <muda/ext/linear_system/csr_matrix_view.h>

namespace muda::details
{
template <typename T, int N>
class MatrixFormatConverter;
}

namespace muda
{
template <typename T>
using DeviceCSRMatrix = DeviceBSRMatrix<T, 1>;
}  // namespace muda
#include "details/device_csr_matrix.inl"
```


