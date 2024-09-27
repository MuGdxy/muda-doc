

# File check.h



[**FileList**](files.md) **>** [**check**](dir_3ada5fb1291f7068cec99adbe813154e.md) **>** [**check.h**](check_8h.md)

[Go to the source code of this file](check_8h_source.md)



* `#include <cuda.h>`
* `#include <cuda_runtime.h>`
* `#include <cuda_runtime_api.h>`
* `#include <cstdio>`
* `#include <muda/muda_def.h>`
* `#include <muda/tools/debug_log.h>`
* `#include <muda/exception.h>`
* `#include <string>`
* `#include <muda/check/check_cusparse.h>`
* `#include <muda/check/check_cublas.h>`
* `#include <muda/check/check_cusolver.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**cuda\_error**](classmuda_1_1cuda__error.md) &lt;typename T&gt;<br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC const char \* | [**mudaCudaGetErrorEnum**](#function-mudacudageterrorenum) (cudaError\_t error) <br> |




























## Public Functions Documentation




### function mudaCudaGetErrorEnum 

```C++
MUDA_INLINE MUDA_GENERIC const char * mudaCudaGetErrorEnum (
    cudaError_t error
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/check/check.h`

