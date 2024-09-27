

# File viewer\_base.h



[**FileList**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**viewer**](dir_b8d9e5dede9d3b62139c9f3b116c88e0.md) **>** [**viewer\_base.h**](viewer__base_8h.md)

[Go to the source code of this file](viewer__base_8h_source.md)



* `#include <cuda.h>`
* `#include <cuda_runtime.h>`
* `#include <cuda_runtime_api.h>`
* `#include <muda/muda_def.h>`
* `#include <muda/tools/debug_log.h>`
* `#include <muda/muda_config.h>`
* `#include <muda/assert.h>`
* `#include <muda/tools/launch_info_cache.h>`
* `#include <muda/tools/fuzzy.h>`
* `#include <muda/type_traits/type_modifier.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**ViewerBase**](classmuda_1_1_viewer_base.md) &lt;IsConst\_&gt;<br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**MUDA\_VIEWER\_COMMON\_NAME**](viewer__base_8h.md#define-muda_viewer_common_name) (viewer\_name) <br> |

## Macro Definition Documentation





### define MUDA\_VIEWER\_COMMON\_NAME 

```C++
#define MUDA_VIEWER_COMMON_NAME (
    viewer_name
) public:                                                                      \
    using this_type = viewer_name;                                             \
                                                                               \
    MUDA_INLINE MUDA_HOST this_type& name(const char* n) noexcept              \
    {                                                                          \ ::muda::ViewerBase <viewer_name::IsConst>::name(n);                     \
        return *this;                                                          \
    }                                                                          \
                                                                               \
    MUDA_INLINE MUDA_GENERIC const char* name() const noexcept                 \
    {                                                                          \
        return ::muda::ViewerBase <viewer_name::IsConst>::name();               \
    }                                                                          \
                                                                               \
  private:
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/viewer/viewer_base.h`

