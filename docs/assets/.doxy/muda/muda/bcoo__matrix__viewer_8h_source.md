

# File bcoo\_matrix\_viewer.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**bcoo\_matrix\_viewer.h**](bcoo__matrix__viewer_8h.md)

[Go to the documentation of this file](bcoo__matrix__viewer_8h.md)


```C++
#pragma once
#include <muda/ext/linear_system/triplet_matrix_viewer.h>
namespace muda
{
template <typename T, int N>
using BCOOMatrixViewer = CTripletMatrixViewer<T, N>;

template <typename T, int N>
using CBCOOMatrixViewer = CTripletMatrixViewer<T, N>;

template <typename T>
using COOMatrixViewer = BCOOMatrixViewer<T, 1>;

template <typename T>
using CCOOMatrixViewer = CBCOOMatrixViewer<T, 1>;
}  // namespace muda

#include "details/bcoo_matrix_viewer.inl"
```


