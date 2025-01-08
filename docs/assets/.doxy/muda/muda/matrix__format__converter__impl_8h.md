

# File matrix\_format\_converter\_impl.h



[**FileList**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**matrix\_format\_converter\_impl.h**](matrix__format__converter__impl_8h.md)

[Go to the source code of this file](matrix__format__converter__impl_8h_source.md)



* `#include <muda/ext/linear_system/linear_system_handles.h>`
* `#include <muda/ext/linear_system/device_dense_matrix.h>`
* `#include <muda/ext/linear_system/device_dense_vector.h>`
* `#include <muda/ext/linear_system/device_triplet_matrix.h>`
* `#include <muda/ext/linear_system/device_doublet_vector.h>`
* `#include <muda/ext/linear_system/device_bcoo_matrix.h>`
* `#include <muda/ext/linear_system/device_bcoo_vector.h>`
* `#include <muda/ext/linear_system/device_bsr_matrix.h>`
* `#include <muda/ext/linear_system/device_csr_matrix.h>`
* `#include <muda/cub/device/device_merge_sort.h>`
* `#include <muda/cub/device/device_radix_sort.h>`
* `#include <muda/cub/device/device_run_length_encode.h>`
* `#include <muda/cub/device/device_scan.h>`
* `#include <muda/cub/device/device_segmented_reduce.h>`
* `#include <muda/cub/device/device_reduce.h>`
* `#include <muda/type_traits/cuda_arch.h>`
* `#include <muda/buffer/device_var.h>`
* `#include <muda/launch.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |
| namespace | [**details**](namespacemuda_1_1details.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**MatrixFormatConverter**](classmuda_1_1details_1_1_matrix_format_converter.md) &lt;typename T, N&gt;<br> |
| class | [**MatrixFormatConverterBase**](classmuda_1_1details_1_1_matrix_format_converter_base.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC constexpr bool | [**operator==**](#function-operator) (const int2 & a, const int2 & b) <br> |




























## Public Functions Documentation




### function operator== 

```C++
MUDA_GENERIC constexpr bool operator== (
    const int2 & a,
    const int2 & b
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/matrix_format_converter_impl.h`

