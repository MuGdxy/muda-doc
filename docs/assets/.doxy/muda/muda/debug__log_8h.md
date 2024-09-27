

# File debug\_log.h



[**FileList**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**debug\_log.h**](debug__log_8h.md)

[Go to the source code of this file](debug__log_8h_source.md)



* `#include <cstdlib>`
* `#include <cassert>`
* `#include <muda/tools/fuzzy.h>`
* `#include <muda/assert.h>`
* `#include <muda/print.h>`
* `#include <muda/muda_config.h>`
* `#include <muda/muda_def.h>`
































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**MUDA\_ASSERT**](debug__log_8h.md#define-muda_assert) (res, fmt, ...) MUDA\_KERNEL\_ASSERT(res, fmt, ##\_\_VA\_ARGS\_\_)<br> |
| define  | [**MUDA\_DEBUG\_TRAP**](debug__log_8h.md#define-muda_debug_trap) () <br> |
| define  | [**MUDA\_ERROR**](debug__log_8h.md#define-muda_error) (fmt, ...) MUDA\_KERNEL\_ERROR(fmt, ##\_\_VA\_ARGS\_\_)<br> |
| define  | [**MUDA\_ERROR\_WITH\_LOCATION**](debug__log_8h.md#define-muda_error_with_location) (fmt, ...) MUDA\_KERNEL\_ERROR\_WITH\_LOCATION(fmt, ##\_\_VA\_ARGS\_\_)<br> |
| define  | [**MUDA\_KERNEL\_ASSERT**](debug__log_8h.md#define-muda_kernel_assert) (res, fmt, ...) <br> |
| define  | [**MUDA\_KERNEL\_CHECK**](debug__log_8h.md#define-muda_kernel_check) (res, fmt, ...) <br> |
| define  | [**MUDA\_KERNEL\_ERROR**](debug__log_8h.md#define-muda_kernel_error) (fmt, ...) <br> |
| define  | [**MUDA\_KERNEL\_ERROR\_WITH\_LOCATION**](debug__log_8h.md#define-muda_kernel_error_with_location) (fmt, ...) <br> |
| define  | [**MUDA\_KERNEL\_PRINT**](debug__log_8h.md#define-muda_kernel_print) (fmt, ...) <br> |
| define  | [**MUDA\_KERNEL\_WARN**](debug__log_8h.md#define-muda_kernel_warn) (fmt, ...) <br> |
| define  | [**MUDA\_KERNEL\_WARN\_WITH\_LOCATION**](debug__log_8h.md#define-muda_kernel_warn_with_location) (fmt, ...) <br> |

## Macro Definition Documentation





### define MUDA\_ASSERT 

```C++
#define MUDA_ASSERT (
    res,
    fmt,
    ...
) MUDA_KERNEL_ASSERT(res, fmt, ##__VA_ARGS__)
```




<hr>



### define MUDA\_DEBUG\_TRAP 

```C++
#define MUDA_DEBUG_TRAP (
    
) {                                                                          \
        if constexpr(::muda::TRAP_ON_ERROR)                                    \
            ::muda::trap();                                                    \
    }
```




<hr>



### define MUDA\_ERROR 

```C++
#define MUDA_ERROR (
    fmt,
    ...
) MUDA_KERNEL_ERROR(fmt, ##__VA_ARGS__)
```




<hr>



### define MUDA\_ERROR\_WITH\_LOCATION 

```C++
#define MUDA_ERROR_WITH_LOCATION (
    fmt,
    ...
) MUDA_KERNEL_ERROR_WITH_LOCATION(fmt, ##__VA_ARGS__)
```




<hr>



### define MUDA\_KERNEL\_ASSERT 

```C++
#define MUDA_KERNEL_ASSERT (
    res,
    fmt,
    ...
) {                                                                             \
        if constexpr(::muda::RUNTIME_CHECK_ON)                                    \
        {                                                                         \
            if(!(res))                                                            \
            {                                                                     \
                MUDA_KERNEL_PRINT("%s(%d): %s:\n <assert> " #res " failed. " fmt, \
                                  __FILE__,                                       \
                                  __LINE__,                                       \
                                  MUDA_FUNCTION_SIG,                              \
                                  ##__VA_ARGS__);                                 \
                MUDA_DEBUG_TRAP();                                                \
            }                                                                     \
        }                                                                         \
    }
```




<hr>



### define MUDA\_KERNEL\_CHECK 

```C++
#define MUDA_KERNEL_CHECK (
    res,
    fmt,
    ...
) {                                                                            \
        if constexpr(::muda::RUNTIME_CHECK_ON)                                   \
        {                                                                        \
            if(!(res))                                                           \
            {                                                                    \
                MUDA_KERNEL_PRINT("%s(%d): %s:\n <check> " #res " failed. " fmt, \
                                  __FILE__,                                      \
                                  __LINE__,                                      \
                                  MUDA_FUNCTION_SIG,                             \
                                  ##__VA_ARGS__);                                \
            }                                                                    \
        }                                                                        \
    }
```




<hr>



### define MUDA\_KERNEL\_ERROR 

```C++
#define MUDA_KERNEL_ERROR (
    fmt,
    ...
) {                                                                          \
        MUDA_KERNEL_PRINT("<error> " fmt, ##__VA_ARGS__);                      \
        MUDA_DEBUG_TRAP();                                                     \
    }
```




<hr>



### define MUDA\_KERNEL\_ERROR\_WITH\_LOCATION 

```C++
#define MUDA_KERNEL_ERROR_WITH_LOCATION (
    fmt,
    ...
) {                                                                                                          \
        MUDA_KERNEL_PRINT("%s(%d): %s:\n <error> " fmt, __FILE__, __LINE__, MUDA_FUNCTION_SIG, ##__VA_ARGS__); \
        MUDA_DEBUG_TRAP();                                                                                     \
    }
```




<hr>



### define MUDA\_KERNEL\_PRINT 

```C++
#define MUDA_KERNEL_PRINT (
    fmt,
    ...
) {                                                                          \
        ::muda::print("(host):" fmt "\n", ##__VA_ARGS__);                      \
    }
```




<hr>



### define MUDA\_KERNEL\_WARN 

```C++
#define MUDA_KERNEL_WARN (
    fmt,
    ...
) {                                                                          \
        MUDA_KERNEL_PRINT("<warn>" fmt, ##__VA_ARGS__);                        \
    }
```




<hr>



### define MUDA\_KERNEL\_WARN\_WITH\_LOCATION 

```C++
#define MUDA_KERNEL_WARN_WITH_LOCATION (
    fmt,
    ...
) {                                                                                                        \
        MUDA_KERNEL_PRINT("%s(%d): %s:\n <warn>" fmt, __FILE__, __LINE__, MUDA_FUNCTION_SIG, ##__VA_ARGS__); \
    }
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/debug_log.h`

