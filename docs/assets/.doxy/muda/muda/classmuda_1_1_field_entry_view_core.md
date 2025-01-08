

# Class muda::FieldEntryViewCore

**template &lt;bool IsConst, typename T, FieldEntryLayout Layout, int M, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldEntryViewCore**](classmuda_1_1_field_entry_view_core.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef typename ViewerCore::ConstMatMap | [**ConstMatMap**](#typedef-constmatmap)  <br> |
| typedef [**CFieldEntryViewer**](classmuda_1_1_c_field_entry_viewer.md)&lt; T, Layout, M, N &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef typename ViewerCore::MatStride | [**MatStride**](#typedef-matstride)  <br> |
| typedef typename ViewerCore::NonConstMatMap | [**NonConstMatMap**](#typedef-nonconstmatmap)  <br> |
| typedef [**FieldEntryViewer**](classmuda_1_1_field_entry_viewer.md)&lt; T, Layout, M, N &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef typename ViewerCore::ThisMatMap | [**ThisMatMap**](#typedef-thismatmap)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_c_field_entry_viewer.md), [**NonConstViewer**](classmuda_1_1_field_entry_viewer.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |


## Public Types inherited from muda::ViewBase

See [muda::ViewBase](classmuda_1_1_view_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_view_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_view_base.md#typedef-non_const_enable_t)  <br> |












## Public Static Attributes inherited from muda::ViewBase

See [muda::ViewBase](classmuda_1_1_view_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_view_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_view_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**FieldEntryViewCore**](#function-fieldentryviewcore-23) () = default<br> |
|  MUDA\_GENERIC | [**FieldEntryViewCore**](#function-fieldentryviewcore-33) ([**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; core, int offset, int size) <br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto | [**elem\_byte\_size**](#function-elem_byte_size) () const<br> |
|  MUDA\_GENERIC auto | [**layout**](#function-layout) () const<br> |
|  MUDA\_GENERIC auto | [**layout\_info**](#function-layout_info) () const<br> |
|  MUDA\_GENERIC auto | [**name**](#function-name) () const<br> |
|  MUDA\_GENERIC auto | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC auto | [**shape**](#function-shape) () const<br> |
|  MUDA\_GENERIC auto | [**size**](#function-size) () const<br> |
|  MUDA\_GENERIC auto | [**struct\_stride**](#function-struct_stride) () const<br> |
|  MUDA\_GENERIC auto | [**total\_count**](#function-total_count) () const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () <br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; | [**m\_core**](#variable-m_core)  <br> |
|  int | [**m\_offset**](#variable-m_offset)   = = 0<br> |
|  int | [**m\_size**](#variable-m_size)   = = 0<br> |
|  MatStride | [**m\_stride**](#variable-m_stride)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**FieldEntryViewCore**](#function-fieldentryviewcore-13) ([**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; core, int offset, int size, [**AsIterator**](structmuda_1_1_field_entry_view_core_1_1_as_iterator.md)) <br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-13) (int i) const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-23) (int i, int j) const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-33) (int i, int row\_index, int col\_index) const<br> |








## Public Types Documentation




### typedef ConstMatMap 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::ConstMatMap =  typename ViewerCore::ConstMatMap;
```




<hr>



### typedef ConstViewer 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::ConstViewer =  CFieldEntryViewer<T, Layout, M, N>;
```




<hr>



### typedef MatStride 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::MatStride =  typename ViewerCore::MatStride;
```




<hr>



### typedef NonConstMatMap 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::NonConstMatMap =  typename ViewerCore::NonConstMatMap;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::NonConstViewer =  FieldEntryViewer<T, Layout, M, N>;
```




<hr>



### typedef ThisMatMap 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::ThisMatMap =  typename ViewerCore::ThisMatMap;
```




<hr>



### typedef ThisViewer 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>



### typedef auto\_const\_t 

```C++
using muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Public Functions Documentation




### function FieldEntryViewCore [2/3]

```C++
MUDA_GENERIC muda::FieldEntryViewCore::FieldEntryViewCore () = default
```




<hr>



### function FieldEntryViewCore [3/3]

```C++
inline MUDA_GENERIC muda::FieldEntryViewCore::FieldEntryViewCore (
    HostDeviceConfigView < FieldEntryCore > core,
    int offset,
    int size
) 
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::cviewer () const
```




<hr>



### function elem\_byte\_size 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::elem_byte_size () const
```




<hr>



### function layout 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::layout () const
```




<hr>



### function layout\_info 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::layout_info () const
```




<hr>



### function name 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::name () const
```




<hr>



### function offset 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::offset () const
```




<hr>



### function shape 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::shape () const
```




<hr>



### function size 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::size () const
```




<hr>



### function struct\_stride 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::struct_stride () const
```




<hr>



### function total\_count 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::total_count () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::FieldEntryViewCore::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_core 

```C++
HostDeviceConfigView<FieldEntryCore> muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::m_core;
```




<hr>



### variable m\_offset 

```C++
int muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::m_offset;
```




<hr>



### variable m\_size 

```C++
int muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::m_size;
```




<hr>



### variable m\_stride 

```C++
MatStride muda::FieldEntryViewCore< IsConst, T, Layout, M, N >::m_stride;
```




<hr>
## Protected Functions Documentation




### function FieldEntryViewCore [1/3]

```C++
inline MUDA_GENERIC muda::FieldEntryViewCore::FieldEntryViewCore (
    HostDeviceConfigView < FieldEntryCore > core,
    int offset,
    int size,
    AsIterator
) 
```




<hr>



### function data [1/3]

```C++
inline MUDA_GENERIC T * muda::FieldEntryViewCore::data (
    int i
) const
```




<hr>



### function data [2/3]

```C++
inline MUDA_GENERIC T * muda::FieldEntryViewCore::data (
    int i,
    int j
) const
```




<hr>



### function data [3/3]

```C++
inline MUDA_GENERIC T * muda::FieldEntryViewCore::data (
    int i,
    int row_index,
    int col_index
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_entry_view.h`

