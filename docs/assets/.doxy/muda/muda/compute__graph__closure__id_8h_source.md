

# File compute\_graph\_closure\_id.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**compute\_graph\_closure\_id.h**](compute__graph__closure__id_8h.md)

[Go to the documentation of this file](compute__graph__closure__id_8h.md)


```C++
#pragma once
#include <muda/tools/id_with_type.h>
namespace muda
{
class ClosureId : public U64IdWithType
{
    using U64IdWithType::U64IdWithType;
};
}  // namespace muda

namespace std
{
template <>
struct hash<muda::ClosureId>
{
    size_t operator()(const muda::ClosureId& s) const noexcept
    {
        return std::hash<uint64_t>{}(s.value());
    }
};
}  // namespace std
```


