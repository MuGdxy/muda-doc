

# File extent.h



[**FileList**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**extent.h**](extent_8h.md)

[Go to the source code of this file](extent_8h_source.md)



* `#include <cuda.h>`
* `#include <muda/muda_def.h>`
* `#include <cinttypes>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**Extent2D**](classmuda_1_1_extent2_d.md) <br> |
| class | [**Extent3D**](classmuda_1_1_extent3_d.md) <br> |
| class | [**Offset2D**](classmuda_1_1_offset2_d.md) <br> |
| class | [**Offset3D**](classmuda_1_1_offset3_d.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**MUDA\_DEFINE\_ARITHMATIC\_OPERATOR**](extent_8h.md#define-muda_define_arithmatic_operator) (op) <br> |
| define  | [**MUDA\_DEFINE\_COMPARISON\_OPERATOR**](extent_8h.md#define-muda_define_comparison_operator) (op) <br> |

## Macro Definition Documentation





### define MUDA\_DEFINE\_ARITHMATIC\_OPERATOR 

```C++
#define MUDA_DEFINE_ARITHMATIC_OPERATOR (
    op
) MUDA_INLINE MUDA_GENERIC Extent2D operator op(const Extent2D& lhs,               \
                                                  const Extent2D& rhs) MUDA_NOEXCEPT \
    {                                                                                \
        return Extent2D{lhs.height() op rhs.height(), lhs.width() op rhs.width()};   \
    }                                                                                \
    MUDA_INLINE MUDA_GENERIC Extent3D operator op(const Extent3D& lhs,               \
                                                  const Extent3D& rhs) MUDA_NOEXCEPT \
    {                                                                                \
        return Extent3D{lhs.depth() op  rhs.depth(),                                 \
                        lhs.height() op rhs.height(),                                \
                        lhs.width() op  rhs.width()};                                 \
    }                                                                                \
    MUDA_INLINE MUDA_GENERIC Offset2D operator op(const Offset2D& lhs,               \
                                                  const Offset2D& rhs) MUDA_NOEXCEPT \
    {                                                                                \
        return Offset2D{lhs.offset_in_height() op rhs.offset_in_height(),            \
                        lhs.offset_in_width() op  rhs.offset_in_width()};             \
    }                                                                                \
    MUDA_INLINE MUDA_GENERIC Offset3D operator op(const Offset3D& lhs,               \
                                                  const Offset3D& rhs) MUDA_NOEXCEPT \
    {                                                                                \
        return Offset3D{lhs.offset_in_depth() op  rhs.offset_in_depth(),             \
                        lhs.offset_in_height() op rhs.offset_in_height(),            \
                        lhs.offset_in_width() op  rhs.offset_in_width()};             \
    }
```




<hr>



### define MUDA\_DEFINE\_COMPARISON\_OPERATOR 

```C++
#define MUDA_DEFINE_COMPARISON_OPERATOR (
    op
) MUDA_INLINE MUDA_GENERIC bool operator op(const Extent2D& lhs, const Extent2D& rhs) MUDA_NOEXCEPT \
    {                                                                                                 \
        return (lhs.height() op rhs.height()) && (lhs.width() op rhs.width());                        \
    }                                                                                                 \
    MUDA_INLINE MUDA_GENERIC bool operator op(const Extent3D& lhs, const Extent3D& rhs) MUDA_NOEXCEPT \
    {                                                                                                 \
        return (lhs.depth() op rhs.depth()) && (lhs.height() op rhs.height())                         \
               && (lhs.width() op rhs.width());                                                       \
    }
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/extent.h`

