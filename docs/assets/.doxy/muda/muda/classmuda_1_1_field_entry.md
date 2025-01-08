

# Class muda::FieldEntry

**template &lt;typename T, FieldEntryLayout Layout, int M, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldEntry**](classmuda_1_1_field_entry.md)








Inherits the following classes: [muda::FieldEntryBase](classmuda_1_1_field_entry_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef typename [**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, Layout, M, N &gt;::ElementType | [**ElementType**](#typedef-elementtype)  <br> |








































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FieldEntry**](#function-fieldentry-12) ([**SubField**](classmuda_1_1_sub_field.md) & field, [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) layout, FieldEntryType type, std::string\_view name) <br> |
|   | [**FieldEntry**](#function-fieldentry-22) ([**SubField**](classmuda_1_1_sub_field.md) & field, [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) layout, FieldEntryType type, uint2 shape, std::string\_view name) <br> |
| virtual void | [**async\_copy\_to\_new\_place**](#function-async_copy_to_new_place) ([**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; new\_place) override const<br> |
|  void | [**copy\_from**](#function-copy_from-13) (const [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; ElementType &gt; & src) <br> |
|  void | [**copy\_from**](#function-copy_from-23) (const std::vector&lt; ElementType &gt; & src) <br> |
|  void | [**copy\_from**](#function-copy_from-33) (const [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, SrcLayout, M, N &gt; & src) <br> |
|  void | [**copy\_to**](#function-copy_to-12) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; ElementType &gt; & dst) const<br> |
|  void | [**copy\_to**](#function-copy_to-22) (std::vector&lt; ElementType &gt; & dst) const<br> |
|  [**CFieldEntryViewer**](classmuda_1_1_c_field_entry_viewer.md)&lt; T, Layout, M, N &gt; | [**cviewer**](#function-cviewer) () const<br> |
|  void | [**fill**](#function-fill) (const ElementType & value) <br> |
|  [**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, Layout, M, N &gt; | [**view**](#function-view-16) () <br> |
|  [**CFieldEntryView**](classmuda_1_1_c_field_entry_view.md)&lt; T, Layout, M, N &gt; | [**view**](#function-view-26) () const<br> |
|  auto | [**view**](#function-view-36) (int offset) <br> |
|  auto | [**view**](#function-view-46) (int offset) const<br> |
|  auto | [**view**](#function-view-56) (int offset, int count) <br> |
|  auto | [**view**](#function-view-66) (int offset, int count) const<br> |
|  [**FieldEntryViewer**](classmuda_1_1_field_entry_viewer.md)&lt; T, Layout, M, N &gt; | [**viewer**](#function-viewer) () <br> |


## Public Functions inherited from muda::FieldEntryBase

See [muda::FieldEntryBase](classmuda_1_1_field_entry_base.md)

| Type | Name |
| ---: | :--- |
|   | [**FieldEntryBase**](classmuda_1_1_field_entry_base.md#function-fieldentrybase-12) ([**SubField**](classmuda_1_1_sub_field.md) & field, [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) layout\_info, FieldEntryType type, uint2 shape, uint32\_t m\_elem\_byte\_size, std::string\_view name) <br> |
|  MUDA\_GENERIC auto | [**count**](classmuda_1_1_field_entry_base.md#function-count) () const<br> |
|  MUDA\_GENERIC auto | [**elem\_byte\_size**](classmuda_1_1_field_entry_base.md#function-elem_byte_size) () const<br> |
|  MUDA\_GENERIC auto | [**layout**](classmuda_1_1_field_entry_base.md#function-layout) () const<br> |
|  MUDA\_GENERIC auto | [**layout\_info**](classmuda_1_1_field_entry_base.md#function-layout_info) () const<br> |
|  MUDA\_GENERIC auto | [**name**](classmuda_1_1_field_entry_base.md#function-name) () const<br> |
|  MUDA\_GENERIC auto | [**shape**](classmuda_1_1_field_entry_base.md#function-shape) () const<br> |
|  MUDA\_GENERIC auto | [**struct\_stride**](classmuda_1_1_field_entry_base.md#function-struct_stride) () const<br> |
|   | [**~FieldEntryBase**](classmuda_1_1_field_entry_base.md#function-fieldentrybase) () = default<br> |
















## Protected Attributes inherited from muda::FieldEntryBase

See [muda::FieldEntryBase](classmuda_1_1_field_entry_base.md)

| Type | Name |
| ---: | :--- |
|  [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) | [**m\_core**](classmuda_1_1_field_entry_base.md#variable-m_core)  <br> |
|  [**SubField**](classmuda_1_1_sub_field.md) & | [**m\_field**](classmuda_1_1_field_entry_base.md#variable-m_field)  <br> |
|  [**HostDeviceConfig**](classmuda_1_1_host_device_config.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; | [**m\_host\_device\_core**](classmuda_1_1_field_entry_base.md#variable-m_host_device_core)  <br> |
|  std::string | [**m\_name**](classmuda_1_1_field_entry_base.md#variable-m_name)  <br> |
































## Protected Functions inherited from muda::FieldEntryBase

See [muda::FieldEntryBase](classmuda_1_1_field_entry_base.md)

| Type | Name |
| ---: | :--- |
|   | [**FieldEntryBase**](classmuda_1_1_field_entry_base.md#function-fieldentrybase-22) (const [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) &) = delete<br> |
| virtual void | [**async\_copy\_to\_new\_place**](classmuda_1_1_field_entry_base.md#function-async_copy_to_new_place) ([**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; vfc) const = 0<br> |
|  MUDA\_GENERIC const auto & | [**core**](classmuda_1_1_field_entry_base.md#function-core) () const<br> |
|  [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) & | [**operator=**](classmuda_1_1_field_entry_base.md#function-operator) (const [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) &) = delete<br> |






## Public Types Documentation




### typedef ElementType 

```C++
using muda::FieldEntry< T, Layout, M, N >::ElementType =  typename FieldEntryView<T, Layout, M, N>::ElementType;
```




<hr>
## Public Functions Documentation




### function FieldEntry [1/2]

```C++
inline muda::FieldEntry::FieldEntry (
    SubField & field,
    FieldEntryLayoutInfo layout,
    FieldEntryType type,
    std::string_view name
) 
```




<hr>



### function FieldEntry [2/2]

```C++
inline muda::FieldEntry::FieldEntry (
    SubField & field,
    FieldEntryLayoutInfo layout,
    FieldEntryType type,
    uint2 shape,
    std::string_view name
) 
```




<hr>



### function async\_copy\_to\_new\_place 

```C++
inline virtual void muda::FieldEntry::async_copy_to_new_place (
    HostDeviceConfigView < FieldEntryCore > new_place
) override const
```



Implements [*muda::FieldEntryBase::async\_copy\_to\_new\_place*](classmuda_1_1_field_entry_base.md#function-async_copy_to_new_place)


<hr>



### function copy\_from [1/3]

```C++
void muda::FieldEntry::copy_from (
    const DeviceBuffer < ElementType > & src
) 
```




<hr>



### function copy\_from [2/3]

```C++
void muda::FieldEntry::copy_from (
    const std::vector< ElementType > & src
) 
```




<hr>



### function copy\_from [3/3]

```C++
template<FieldEntryLayout SrcLayout>
void muda::FieldEntry::copy_from (
    const FieldEntry < T, SrcLayout, M, N > & src
) 
```




<hr>



### function copy\_to [1/2]

```C++
void muda::FieldEntry::copy_to (
    DeviceBuffer < ElementType > & dst
) const
```




<hr>



### function copy\_to [2/2]

```C++
void muda::FieldEntry::copy_to (
    std::vector< ElementType > & dst
) const
```




<hr>



### function cviewer 

```C++
inline CFieldEntryViewer < T, Layout, M, N > muda::FieldEntry::cviewer () const
```




<hr>



### function fill 

```C++
void muda::FieldEntry::fill (
    const ElementType & value
) 
```




<hr>



### function view [1/6]

```C++
inline FieldEntryView < T, Layout, M, N > muda::FieldEntry::view () 
```




<hr>



### function view [2/6]

```C++
inline CFieldEntryView < T, Layout, M, N > muda::FieldEntry::view () const
```




<hr>



### function view [3/6]

```C++
inline auto muda::FieldEntry::view (
    int offset
) 
```




<hr>



### function view [4/6]

```C++
inline auto muda::FieldEntry::view (
    int offset
) const
```




<hr>



### function view [5/6]

```C++
inline auto muda::FieldEntry::view (
    int offset,
    int count
) 
```




<hr>



### function view [6/6]

```C++
inline auto muda::FieldEntry::view (
    int offset,
    int count
) const
```




<hr>



### function viewer 

```C++
inline FieldEntryViewer < T, Layout, M, N > muda::FieldEntry::viewer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field.h`

