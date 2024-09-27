

# File logger\_viewer.h



[**FileList**](files.md) **>** [**logger**](dir_7d83e812141fe1e865a4aab383f85074.md) **>** [**logger\_viewer.h**](logger__viewer_8h.md)

[Go to the source code of this file](logger__viewer_8h_source.md)



* `#include <muda/logger/logger_basic_data.h>`
* `#include <muda/muda_def.h>`
* `#include <muda/check/check_cuda_errors.h>`
* `#include <muda/literal/unit.h>`
* `#include <muda/viewer/dense.h>`
* `#include <muda/logger/details/logger_viewer.inl>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**LogProxy**](classmuda_1_1_log_proxy.md) <br> |
| class | [**LoggerViewer**](classmuda_1_1_logger_viewer.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**PROXY\_OPERATOR**](logger__viewer_8h.md#define-proxy_operator) (enum\_name, T) <br> |

## Macro Definition Documentation





### define PROXY\_OPERATOR 

```C++
#define PROXY_OPERATOR (
    enum_name,
    T
) MUDA_INLINE MUDA_DEVICE friend LogProxy operator<<(LogProxy p, T v)        \
    {                                                                          \
        details::LoggerMetaData meta;                                          \
        meta.type = LoggerBasicType::enum_name;                                \
        meta.size = sizeof(T);                                                 \
        meta.id   = p.m_log_id;                                                \
        p.push_data(meta, &v);                                                 \
        return p;                                                              \
    }
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/logger/logger_viewer.h`

