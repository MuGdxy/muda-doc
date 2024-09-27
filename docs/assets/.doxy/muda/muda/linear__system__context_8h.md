

# File linear\_system\_context.h



[**FileList**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**linear\_system\_context.h**](linear__system__context_8h.md)

[Go to the source code of this file](linear__system__context_8h_source.md)



* `#include <cublas_v2.h>`
* `#include <cusparse_v2.h>`
* `#include <cusolverDn.h>`
* `#include <cusolverSp.h>`
* `#include <list>`
* `#include <muda/buffer/device_buffer.h>`
* `#include <muda/literal/unit.h>`
* `#include <muda/mstl/span.h>`
* `#include <muda/ext/linear_system/dense_vector_view.h>`
* `#include <muda/ext/linear_system/dense_matrix_view.h>`
* `#include <muda/ext/linear_system/matrix_format_converter.h>`
* `#include <muda/ext/linear_system/linear_system_handles.h>`
* `#include <muda/ext/linear_system/linear_system_solve_tolerance.h>`
* `#include <muda/ext/linear_system/linear_system_solve_reorder.h>`
* `#include "details/linear_system_context.inl"`
* `#include "details/routines/convert.inl"`
* `#include "details/routines/norm.inl"`
* `#include "details/routines/dot.inl"`
* `#include "details/routines/axpby.inl"`
* `#include "details/routines/spmv.inl"`
* `#include "details/routines/mv.inl"`
* `#include "details/routines/solve.inl"`
* `#include "details/routines/mm.inl"`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**LinearSystemContext**](classmuda_1_1_linear_system_context.md) <br> |
| class | [**LinearSystemContextCreateInfo**](classmuda_1_1_linear_system_context_create_info.md) <br> |



















































------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/linear_system_context.h`

