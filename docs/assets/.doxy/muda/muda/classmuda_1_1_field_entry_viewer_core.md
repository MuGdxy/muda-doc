

# Class muda::FieldEntryViewerCore

**template &lt;bool IsConst, typename T, FieldEntryLayout Layout, int M, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldEntryViewerCore**](classmuda_1_1_field_entry_viewer_core.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Map&lt; const Eigen::Matrix&lt; T, M, N &gt;, 0, MatStride &gt; | [**ConstMatMap**](#typedef-constmatmap)  <br> |
| typedef details::field::MatStride | [**MatStride**](#typedef-matstride)  <br> |
| typedef Eigen::Map&lt; Eigen::Matrix&lt; T, M, N &gt;, 0, MatStride &gt; | [**NonConstMatMap**](#typedef-nonconstmatmap)  <br> |
| typedef std::conditional\_t&lt; IsConst, ConstMatMap, NonConstMatMap &gt; | [**ThisMatMap**](#typedef-thismatmap)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**FieldEntryViewerCore**](#function-fieldentryviewercore-13) () <br> |
|  MUDA\_GENERIC | [**FieldEntryViewerCore**](#function-fieldentryviewercore-23) ([**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; core, int offset, int size) <br> |
|  MUDA\_GENERIC | [**FieldEntryViewerCore**](#function-fieldentryviewercore-33) (const [**FieldEntryViewerCore**](classmuda_1_1_field_entry_viewer_core.md) &) = default<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-13) (int i) const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-23) (int i, int j) const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-33) (int i, int row\_index, int col\_index) const<br> |
|  MUDA\_GENERIC auto | [**elem\_byte\_size**](#function-elem_byte_size) () const<br> |
|  MUDA\_GENERIC auto | [**entry\_name**](#function-entry_name) () const<br> |
|  MUDA\_GENERIC auto | [**layout**](#function-layout) () const<br> |
|  MUDA\_GENERIC auto | [**layout\_info**](#function-layout_info) () const<br> |
|  MUDA\_GENERIC auto | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC auto | [**shape**](#function-shape) () const<br> |
|  MUDA\_GENERIC auto | [**size**](#function-size) () const<br> |
|  MUDA\_GENERIC auto | [**struct\_stride**](#function-struct_stride) () const<br> |
|  MUDA\_GENERIC auto | [**total\_count**](#function-total_count) () const<br> |


## Public Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-13) () <br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-23) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-33) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**copy\_label**](classmuda_1_1_viewer_base.md#function-copy_label) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) & other) <br> |
|  MUDA\_GENERIC const char \* | [**kernel\_file**](classmuda_1_1_viewer_base.md#function-kernel_file) () const<br> |
|  MUDA\_GENERIC int | [**kernel\_line**](classmuda_1_1_viewer_base.md#function-kernel_line) () const<br> |
|  MUDA\_GENERIC const char \* | [**kernel\_name**](classmuda_1_1_viewer_base.md#function-kernel_name) () const<br> |
|  MUDA\_GENERIC const char \* | [**name**](classmuda_1_1_viewer_base.md#function-name-13) () const<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator_1) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |






## Protected Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |


## Protected Types inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_viewer_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_viewer_base.md#typedef-non_const_enable_t)  <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; | [**m\_core**](#variable-m_core)  <br> |
|  int | [**m\_offset**](#variable-m_offset)   = = 0<br> |
|  int | [**m\_size**](#variable-m_size)   = = 0<br> |
|  MatStride | [**m\_stride**](#variable-m_stride)  <br> |


































## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef ConstMatMap 

```C++
using muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::ConstMatMap =  Eigen::Map<const Eigen::Matrix<T, M, N>, 0, MatStride>;
```




<hr>



### typedef MatStride 

```C++
using muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::MatStride =  details::field::MatStride;
```




<hr>



### typedef NonConstMatMap 

```C++
using muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::NonConstMatMap =  Eigen::Map<Eigen::Matrix<T, M, N>, 0, MatStride>;
```




<hr>



### typedef ThisMatMap 

```C++
using muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::ThisMatMap =  std::conditional_t<IsConst, ConstMatMap, NonConstMatMap>;
```




<hr>
## Public Functions Documentation




### function FieldEntryViewerCore [1/3]

```C++
inline MUDA_GENERIC muda::FieldEntryViewerCore::FieldEntryViewerCore () 
```




<hr>



### function FieldEntryViewerCore [2/3]

```C++
inline MUDA_GENERIC muda::FieldEntryViewerCore::FieldEntryViewerCore (
    HostDeviceConfigView < FieldEntryCore > core,
    int offset,
    int size
) 
```




<hr>



### function FieldEntryViewerCore [3/3]

```C++
MUDA_GENERIC muda::FieldEntryViewerCore::FieldEntryViewerCore (
    const FieldEntryViewerCore &
) = default
```




<hr>



### function data [1/3]

```C++
inline MUDA_GENERIC T * muda::FieldEntryViewerCore::data (
    int i
) const
```




<hr>



### function data [2/3]

```C++
inline MUDA_GENERIC T * muda::FieldEntryViewerCore::data (
    int i,
    int j
) const
```




<hr>



### function data [3/3]

```C++
inline MUDA_GENERIC T * muda::FieldEntryViewerCore::data (
    int i,
    int row_index,
    int col_index
) const
```




<hr>



### function elem\_byte\_size 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::elem_byte_size () const
```




<hr>



### function entry\_name 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::entry_name () const
```




<hr>



### function layout 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::layout () const
```




<hr>



### function layout\_info 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::layout_info () const
```




<hr>



### function offset 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::offset () const
```




<hr>



### function shape 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::shape () const
```




<hr>



### function size 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::size () const
```




<hr>



### function struct\_stride 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::struct_stride () const
```




<hr>



### function total\_count 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewerCore::total_count () const
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_core 

```C++
HostDeviceConfigView<FieldEntryCore> muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::m_core;
```




<hr>



### variable m\_offset 

```C++
int muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::m_offset;
```




<hr>



### variable m\_size 

```C++
int muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::m_size;
```




<hr>



### variable m\_stride 

```C++
MatStride muda::FieldEntryViewerCore< IsConst, T, Layout, M, N >::m_stride;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_entry_viewer.h`

