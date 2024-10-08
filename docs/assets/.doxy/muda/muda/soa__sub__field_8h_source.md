

# File soa\_sub\_field.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**field**](dir_67616bafb1e973d10aec465c6be4ad46.md) **>** [**sub\_field**](dir_d0784a59e778fb60ba75a554135ad43c.md) **>** [**soa\_sub\_field.h**](soa__sub__field_8h.md)

[Go to the documentation of this file](soa__sub__field_8h.md)


```C++
#pragma once
#include <muda/ext/field/sub_field_interface.h>

namespace muda
{
namespace details
{
    struct SoACopyMap
    {
        uint32_t offset_in_base_struct;
        uint32_t elem_byte_size;
    };
}  // namespace details


template <>
class SubFieldImpl<FieldEntryLayout::SoA> : public SubFieldInterface
{
    friend class SubField;

    DeviceBuffer<details::SoACopyMap> m_copy_map_buffer;
    std::vector<details::SoACopyMap>  m_h_copy_map_buffer;
    uint32_t                          m_base_struct_stride = ~0;

  protected:
    virtual void build_impl() override;
    virtual size_t require_total_buffer_byte_size(size_t element_count) override;
    virtual void calculate_new_cores(std::byte*           byte_buffer,
                                     size_t               total_bytes,
                                     size_t               element_count,
                                     span<FieldEntryCore> new_cores) override;
    virtual bool allow_inplace_shrink() const { return false; }

  public:
    using SubFieldInterface::SubFieldInterface;
    virtual ~SubFieldImpl() override = default;
};
}  // namespace muda

#include "details/soa_sub_field.inl"
```


