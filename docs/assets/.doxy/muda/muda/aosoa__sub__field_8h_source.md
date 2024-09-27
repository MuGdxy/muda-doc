

# File aosoa\_sub\_field.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**field**](dir_67616bafb1e973d10aec465c6be4ad46.md) **>** [**sub\_field**](dir_d0784a59e778fb60ba75a554135ad43c.md) **>** [**aosoa\_sub\_field.h**](aosoa__sub__field_8h.md)

[Go to the documentation of this file](aosoa__sub__field_8h.md)


```C++
#pragma once
#include <muda/ext/field/sub_field_interface.h>

namespace muda
{
template <>
class SubFieldImpl<FieldEntryLayout::AoSoA> : public SubFieldInterface
{
    friend class SubField;

  protected:
    virtual void build_impl() override;

    virtual size_t require_total_buffer_byte_size(size_t element_count) override;
    virtual void calculate_new_cores(std::byte*           byte_buffer,
                                     size_t               total_bytes,
                                     size_t               element_count,
                                     span<FieldEntryCore> new_cores) override
    {
        // no need to update any other thing
    }


  public:
    using SubFieldInterface::SubFieldInterface;
    virtual ~SubFieldImpl() override = default;
};

}  // namespace muda

#include "details/aosoa_sub_field.inl"
```


