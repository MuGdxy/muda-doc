

# File algo\_mapper.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**type\_mapper**](dir_409feac54749c96b1f5e03ed3e08c376.md) **>** [**algo\_mapper.h**](algo__mapper_8h.md)

[Go to the documentation of this file](algo__mapper_8h.md)


```C++
#pragma once
#include <cublas_v2.h>
#include <cusparse_v2.h>
#include <muda/type_traits/always.h>
namespace muda
{
class LinearSystemAlgorithm
{
  public:
    // convert for compatibility
    constexpr static cusparseSpMVAlg_t SPMV_ALG_DEFAULT = (cusparseSpMVAlg_t)0;
};
}  // namespace muda
```


