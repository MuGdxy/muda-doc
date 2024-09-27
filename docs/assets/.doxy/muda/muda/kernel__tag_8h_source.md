

# File kernel\_tag.h

[**File List**](files.md) **>** [**launch**](dir_440d6ef7395341c98b5d944289d06a83.md) **>** [**kernel\_tag.h**](kernel__tag_8h.md)

[Go to the documentation of this file](kernel__tag_8h.md)


```C++
#pragma once
namespace muda
{
template <typename T>
struct Tag
{
};

struct Default
{
};

using DefaultTag = Tag<Default>;
}  // namespace muda
```


