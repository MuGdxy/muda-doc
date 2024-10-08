

# File sub\_field.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**field**](dir_67616bafb1e973d10aec465c6be4ad46.md) **>** [**sub\_field.h**](sub__field_8h.md)

[Go to the documentation of this file](sub__field_8h.md)


```C++
#pragma once
#include <memory>
#include <muda/tools/host_device_string_cache.h>
#include <muda/ext/field/field_build_options.h>
#include <muda/buffer/device_buffer.h>
#include <muda/ext/field/field_entry_type.h>
#include <muda/ext/field/field_builder.h>

namespace muda
{
class Field;
class FieldEntryBase;
template <typename T, FieldEntryLayout Layout, int M, int N>
class FieldEntry;
class SubFieldInterface;

class SubField
{
    template <typename T>
    using U = std::unique_ptr<T>;

    Field&               m_field;
    std::string          m_name;
    U<SubFieldInterface> m_interface;
    bool                 m_is_built = false;

    std::byte* data_buffer() const;
    size_t     num_entries() const;

    FieldEntryBase* find_entry(std::string_view name) const;

    template <typename FieldEntryT>
    FieldEntryT* find_entry(std::string_view name) const;

  public:
    SubField(Field& field, std::string_view name);
    ~SubField();

    std::string_view name() const { return m_name; }

    size_t size() const;
    void   resize(size_t num_elements);

    template <FieldEntryLayout Layout>
    FieldBuilder<Layout> builder(FieldEntryLayoutInfo layout = FieldEntryLayoutInfo{Layout},
                                 const FieldBuildOptions& options = {});
    FieldBuilder<FieldEntryLayout::RuntimeLayout> builder(FieldEntryLayoutInfo layout,
                                                          const FieldBuildOptions& options = {});
    FieldBuilder<FieldEntryLayout::AoSoA> AoSoA(uint32_t innermost_array_size = 32,
                                                const FieldBuildOptions& options = {});
    FieldBuilder<FieldEntryLayout::SoA> SoA(const FieldBuildOptions& options = {});
    FieldBuilder<FieldEntryLayout::AoS> AoS(const FieldBuildOptions& options = {});

    // delete copy and move
    SubField(const SubField&)            = delete;
    SubField(SubField&&)                 = delete;
    SubField& operator=(const SubField&) = delete;
    SubField& operator=(SubField&&)      = delete;

  private:
    friend class Field;
    friend class SubField;
    template <FieldEntryLayout Layout>
    friend class FieldBuilder;
    friend class FieldEntryBase;
    template <typename T, FieldEntryLayout Layout, int M, int N>
    friend class FieldEntry;

    template <typename T, FieldEntryLayout Layout, int M, int N>
    FieldEntry<T, Layout, M, N>& create_entry(std::string_view     name,
                                              FieldEntryLayoutInfo layout,
                                              FieldEntryType       type,
                                              uint2                shape);

    void build(const FieldBuildOptions& options);
    bool allow_inplace_shrink() const;
};
}  // namespace muda

#include "details/sub_field.inl"
```


