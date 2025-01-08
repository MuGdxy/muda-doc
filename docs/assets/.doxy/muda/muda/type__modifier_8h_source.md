

# File type\_modifier.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**type\_traits**](dir_604bea9d06d02462c18f7966e507987c.md) **>** [**type\_modifier.h**](type__modifier_8h.md)

[Go to the documentation of this file](type__modifier_8h.md)


```C++
#pragma once
#include <type_traits>
#include <muda/muda_def.h>

namespace muda
{
/*************************************************************************
* 
*                               Raw Type
* 
*************************************************************************/
template <typename T>
using raw_type_t = std::remove_all_extents_t<std::remove_reference_t<T>>;

/*************************************************************************
* 
*                               View Type
* 
*************************************************************************/
template <typename T>
struct read_only_view
{
    using type = T;
};

template <typename T>
struct read_write_view
{
    using type = T;
};

template <typename T>
using read_only_view_t = typename read_only_view<T>::type;

template <typename T>
constexpr bool is_read_only_view_v = std::is_same_v<T, read_only_view_t<T>>;

template <typename T>
using read_write_view_t = typename read_write_view<T>::type;

template <typename T>
constexpr bool is_read_write_view_v = std::is_same_v<T, read_write_view_t<T>>;

template <typename T>
constexpr bool is_uniform_view_v = is_read_only_view_v<T> && is_read_write_view_v<T>;

/*************************************************************************
* 
*                           Remove Const
* 
*************************************************************************/
template <typename T>
MUDA_GENERIC MUDA_INLINE constexpr T* remove_const(const T* ptr) noexcept
{
    return const_cast<T*>(ptr);
}

template <typename T>
MUDA_GENERIC MUDA_INLINE constexpr T& remove_const(const T& ref) noexcept
{
    return const_cast<T&>(ref);
}
}  // namespace muda
```


