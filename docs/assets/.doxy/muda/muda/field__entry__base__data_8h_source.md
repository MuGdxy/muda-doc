

# File field\_entry\_base\_data.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**field**](dir_67616bafb1e973d10aec465c6be4ad46.md) **>** [**field\_entry\_base\_data.h**](field__entry__base__data_8h.md)

[Go to the documentation of this file](field__entry__base__data_8h.md)


```C++
#pragma once
#include <muda/ext/field/field_entry_type.h>
#include <muda/ext/field/field_entry_layout.h>
namespace muda
{
class FieldEntryBaseData
{
  public:
    // common info
    FieldEntryLayoutInfo layout_info;
    FieldEntryType       type = FieldEntryType::None;
    uint2                shape;
    uint32_t             elem_byte_size = ~0;
    //uint32_t             elem_alignment   = ~0;
    uint32_t elem_count       = ~0;
    uint32_t offset_in_struct = ~0;

    // used by soa
    uint32_t offset_in_base_struct = ~0;
    union
    {
        // used by aos and aosoa
        uint32_t struct_stride = ~0;
        // used by soa
        uint32_t elem_count_based_stride;
    };
};
}  // namespace muda
```


