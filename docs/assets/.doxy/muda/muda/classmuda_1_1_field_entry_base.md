

# Class muda::FieldEntryBase



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldEntryBase**](classmuda_1_1_field_entry_base.md)










Inherited by the following classes: [muda::FieldEntry](classmuda_1_1_field_entry.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FieldEntryBase**](#function-fieldentrybase-12) ([**SubField**](classmuda_1_1_sub_field.md) & field, [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) layout\_info, FieldEntryType type, uint2 shape, uint32\_t m\_elem\_byte\_size, std::string\_view name) <br> |
|  MUDA\_GENERIC auto | [**count**](#function-count) () const<br> |
|  MUDA\_GENERIC auto | [**elem\_byte\_size**](#function-elem_byte_size) () const<br> |
|  MUDA\_GENERIC auto | [**layout**](#function-layout) () const<br> |
|  MUDA\_GENERIC auto | [**layout\_info**](#function-layout_info) () const<br> |
|  MUDA\_GENERIC auto | [**name**](#function-name) () const<br> |
|  MUDA\_GENERIC auto | [**shape**](#function-shape) () const<br> |
|  MUDA\_GENERIC auto | [**struct\_stride**](#function-struct_stride) () const<br> |
|   | [**~FieldEntryBase**](#function-fieldentrybase) () = default<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) | [**m\_core**](#variable-m_core)  <br> |
|  [**SubField**](classmuda_1_1_sub_field.md) & | [**m\_field**](#variable-m_field)  <br> |
|  [**HostDeviceConfig**](classmuda_1_1_host_device_config.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; | [**m\_host\_device\_core**](#variable-m_host_device_core)  <br> |
|  std::string | [**m\_name**](#variable-m_name)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**FieldEntryBase**](#function-fieldentrybase-22) (const [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) &) = delete<br> |
| virtual void | [**async\_copy\_to\_new\_place**](#function-async_copy_to_new_place) ([**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; vfc) const = 0<br> |
|  MUDA\_GENERIC const auto & | [**core**](#function-core) () const<br> |
|  [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) & | [**operator=**](#function-operator) (const [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) &) = delete<br> |




## Public Functions Documentation




### function FieldEntryBase [1/2]

```C++
inline muda::FieldEntryBase::FieldEntryBase (
    SubField & field,
    FieldEntryLayoutInfo layout_info,
    FieldEntryType type,
    uint2 shape,
    uint32_t m_elem_byte_size,
    std::string_view name
) 
```




<hr>



### function count 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::count () const
```




<hr>



### function elem\_byte\_size 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::elem_byte_size () const
```




<hr>



### function layout 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::layout () const
```




<hr>



### function layout\_info 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::layout_info () const
```




<hr>



### function name 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::name () const
```




<hr>



### function shape 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::shape () const
```




<hr>



### function struct\_stride 

```C++
inline MUDA_GENERIC auto muda::FieldEntryBase::struct_stride () const
```




<hr>



### function ~FieldEntryBase 

```C++
muda::FieldEntryBase::~FieldEntryBase () = default
```




<hr>
## Protected Attributes Documentation




### variable m\_core 

```C++
FieldEntryCore muda::FieldEntryBase::m_core;
```




<hr>



### variable m\_field 

```C++
SubField& muda::FieldEntryBase::m_field;
```




<hr>



### variable m\_host\_device\_core 

```C++
HostDeviceConfig<FieldEntryCore> muda::FieldEntryBase::m_host_device_core;
```




<hr>



### variable m\_name 

```C++
std::string muda::FieldEntryBase::m_name;
```




<hr>
## Protected Functions Documentation




### function FieldEntryBase [2/2]

```C++
muda::FieldEntryBase::FieldEntryBase (
    const FieldEntryBase &
) = delete
```




<hr>



### function async\_copy\_to\_new\_place 

```C++
virtual void muda::FieldEntryBase::async_copy_to_new_place (
    HostDeviceConfigView < FieldEntryCore > vfc
) const = 0
```




<hr>



### function core 

```C++
inline MUDA_GENERIC const auto & muda::FieldEntryBase::core () const
```




<hr>



### function operator= 

```C++
FieldEntryBase & muda::FieldEntryBase::operator= (
    const FieldEntryBase &
) = delete
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_entry.h`

