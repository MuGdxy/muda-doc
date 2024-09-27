

# File always.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**type\_traits**](dir_604bea9d06d02462c18f7966e507987c.md) **>** [**always.h**](always_8h.md)

[Go to the documentation of this file](always_8h.md)


```C++
#pragma once

namespace muda
{
template <typename T>
struct always_false
{
    static constexpr bool value = false;
};

template <typename T>
constexpr bool always_false_v = always_false<T>::value;

template <typename T>
struct always_true
{
    static constexpr bool value = true;
};
}  // namespace muda
```


