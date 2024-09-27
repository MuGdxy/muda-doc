

# File field\_build\_options.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**field**](dir_67616bafb1e973d10aec465c6be4ad46.md) **>** [**field\_build\_options.h**](field__build__options_8h.md)

[Go to the documentation of this file](field__build__options_8h.md)


```C++
#pragma once
#include <muda/ext/field/field_entry_layout.h>
namespace muda
{
class FieldBuildOptions
{
  public:
    uint32_t min_alignment = sizeof(int);  // bytes
    uint32_t max_alignment = sizeof(std::max_align_t);
};
}  // namespace muda
```


