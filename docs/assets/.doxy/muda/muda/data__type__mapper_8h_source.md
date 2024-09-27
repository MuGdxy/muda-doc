

# File data\_type\_mapper.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**type\_mapper**](dir_409feac54749c96b1f5e03ed3e08c376.md) **>** [**data\_type\_mapper.h**](data__type__mapper_8h.md)

[Go to the documentation of this file](data__type__mapper_8h.md)


```C++
#pragma once
#include <cublas_v2.h>
#include <cusparse_v2.h>
#include <muda/type_traits/always.h>
namespace muda
{
template <typename T>
inline constexpr cudaDataType_t cuda_data_type()
{
    if constexpr(std::is_same_v<T, float>)
    {
        return CUDA_R_32F;
    }
    else if constexpr(std::is_same_v<T, double>)
    {
        return CUDA_R_64F;
    }
    else if constexpr(std::is_same_v<T, cuComplex>)
    {
        return CUDA_C_32F;
    }
    else if constexpr(std::is_same_v<T, cuDoubleComplex>)
    {
        return CUDA_C_64F;
    }
    else
    {
        static_assert(always_false_v<T>, "not supported type");
    }
}

constexpr cublasOperation_t cublas_trans_operation(bool b)
{
    return b ? CUBLAS_OP_T : CUBLAS_OP_N;
}

template <typename T>
constexpr cusparseIndexType_t cusparse_index_type()
{
    if constexpr(std::is_same_v<T, int>)
        return cusparseIndexType_t::CUSPARSE_INDEX_32I;
    else if constexpr(std::is_same_v<T, int64_t>)
        return cusparseIndexType_t::CUSPARSE_INDEX_64I;
    else if constexpr(std::is_same_v<T, uint16_t>)
        return cusparseIndexType_t::CUSPARSE_INDEX_16U;
    else
        static_assert(always_false_v<T>, "Unsupported type");
}
}  // namespace muda
```


