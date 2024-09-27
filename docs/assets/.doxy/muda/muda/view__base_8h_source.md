

# File view\_base.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**view**](dir_db2dafed41077e2be62453d93935ca4c.md) **>** [**view\_base.h**](view__base_8h.md)

[Go to the documentation of this file](view__base_8h.md)


```C++
#pragma once
#include <muda/type_traits/type_modifier.h>

namespace muda
{
template <bool IsConst_>
class ViewBase
{
  public:
    constexpr static bool IsConst    = IsConst_;
    constexpr static bool IsNonConst = !IsConst_;
    template <typename T>
    using auto_const_t = std::conditional_t<IsConst, const T, T>;
    template <typename T>
    using non_const_enable_t = std::enable_if_t<IsNonConst, T>;

  private:
    std::byte _dummy; // a workaround to avoid NVCC EBO bug.
};
}  // namespace muda
```


