

# File check\_cusparse.h

[**File List**](files.md) **>** [**check**](dir_3ada5fb1291f7068cec99adbe813154e.md) **>** [**check\_cusparse.h**](check__cusparse_8h.md)

[Go to the documentation of this file](check__cusparse_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <cusparse.h>


MUDA_INLINE MUDA_GENERIC const char* mudaCudaGetErrorEnum(cusparseStatus_t error)
{
    switch(error)
    {
        case CUSPARSE_STATUS_SUCCESS:
            return "CUSPARSE_STATUS_SUCCESS";

        case CUSPARSE_STATUS_NOT_INITIALIZED:
            return "CUSPARSE_STATUS_NOT_INITIALIZED";

        case CUSPARSE_STATUS_ALLOC_FAILED:
            return "CUSPARSE_STATUS_ALLOC_FAILED";

        case CUSPARSE_STATUS_INVALID_VALUE:
            return "CUSPARSE_STATUS_INVALID_VALUE";

        case CUSPARSE_STATUS_ARCH_MISMATCH:
            return "CUSPARSE_STATUS_ARCH_MISMATCH";

        case CUSPARSE_STATUS_MAPPING_ERROR:
            return "CUSPARSE_STATUS_MAPPING_ERROR";

        case CUSPARSE_STATUS_EXECUTION_FAILED:
            return "CUSPARSE_STATUS_EXECUTION_FAILED";

        case CUSPARSE_STATUS_INTERNAL_ERROR:
            return "CUSPARSE_STATUS_INTERNAL_ERROR";

        case CUSPARSE_STATUS_MATRIX_TYPE_NOT_SUPPORTED:
            return "CUSPARSE_STATUS_MATRIX_TYPE_NOT_SUPPORTED";
    }

    return "<unknown>";
}
```


