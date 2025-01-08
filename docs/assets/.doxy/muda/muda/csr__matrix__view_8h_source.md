

# File csr\_matrix\_view.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**csr\_matrix\_view.h**](csr__matrix__view_8h.md)

[Go to the documentation of this file](csr__matrix__view_8h.md)


```C++
#pragma once
#include <muda/ext/linear_system/common.h>
#include <muda/view/view_base.h>
#include <muda/ext/linear_system/bsr_matrix_view.h>

namespace muda
{
template <bool IsConst, typename Ty>
using CSRMatrixViewT = BSRMatrixViewT<IsConst, Ty, 1>;

template <typename Ty>
using CSRMatrixView = CSRMatrixViewT<false, Ty>;
template <typename Ty>
using CCSRMatrixView = CSRMatrixViewT<true, Ty>;
}  // namespace muda

#include "details/csr_matrix_view.inl"
```


