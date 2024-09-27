

# Class muda::Buffer3DViewT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**CDense3D**](classmuda_1_1_dense3_d_base.md)&lt; T &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)&lt; false, T &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)&lt;!IsConst, T &gt; | [**OtherView**](#typedef-otherview)  <br> |
| typedef [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_dense3_d_base.md), [**Viewer**](classmuda_1_1_dense3_d_base.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**Dense3D**](classmuda_1_1_dense3_d_base.md)&lt; T &gt; | [**Viewer**](#typedef-viewer)  <br> |


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
|  constexpr bool | [**IsConst**](classmuda_1_1_view_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_view_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Buffer3DViewT**](#function-buffer3dviewt-26) () <br> |
|  MUDA\_GENERIC | [**Buffer3DViewT**](#function-buffer3dviewt-36) (const [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md) &) <br> |
|  MUDA\_GENERIC | [**Buffer3DViewT**](#function-buffer3dviewt-46) (const [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC | [**Buffer3DViewT**](#function-buffer3dviewt-56) (auto\_const\_t&lt; T &gt; \* data, size\_t pitch\_bytes, size\_t pitch\_bytes\_area, size\_t origin\_width, size\_t origin\_height, const [**Offset3D**](classmuda_1_1_offset3_d.md) & offset, const [**Extent3D**](classmuda_1_1_extent3_d.md) & extent) <br> |
|  MUDA\_GENERIC | [**Buffer3DViewT**](#function-buffer3dviewt-66) (T \* data, size\_t pitch\_bytes, size\_t pitch\_bytes\_area, const [**Offset3D**](classmuda_1_1_offset3_d.md) & offset, const [**Extent3D**](classmuda_1_1_extent3_d.md) & extent) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_buffer3_d_view_t.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-12) (const [**Buffer3DViewT**](classmuda_1_1_buffer3_d_view_t.md)&lt; true, T &gt; & other) const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-22) (const T \* host) const<br> |
|  MUDA\_HOST void | [**copy\_to**](#function-copy_to) (T \* host) const<br> |
|  MUDA\_GENERIC [**CViewer**](classmuda_1_1_dense3_d_base.md) | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-12) (size\_t x, size\_t y, size\_t z) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-22) (size\_t flatten\_i) const<br> |
|  MUDA\_GENERIC [**Extent3D**](classmuda_1_1_extent3_d.md) | [**extent**](#function-extent) () const<br> |
|  MUDA\_HOST void | [**fill**](#function-fill) (const T & v) const<br> |
|  MUDA\_GENERIC [**Offset3D**](classmuda_1_1_offset3_d.md) | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**origin\_data**](#function-origin_data) () const<br> |
|  MUDA\_GENERIC size\_t | [**pitch\_bytes**](#function-pitch_bytes) () const<br> |
|  MUDA\_GENERIC size\_t | [**pitch\_bytes\_area**](#function-pitch_bytes_area) () const<br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_buffer3_d_view_t.md) | [**subview**](#function-subview) ([**Offset3D**](classmuda_1_1_offset3_d.md) offset, [**Extent3D**](classmuda_1_1_extent3_d.md) extent={}) const<br> |
|  MUDA\_GENERIC size\_t | [**total\_size**](#function-total_size) () const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](#function-viewer) () const<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |
|  [**Extent3D**](classmuda_1_1_extent3_d.md) | [**m\_extent**](#variable-m_extent)  <br> |
|  [**Offset3D**](classmuda_1_1_offset3_d.md) | [**m\_offset**](#variable-m_offset)  <br> |
|  size\_t | [**m\_origin\_height**](#variable-m_origin_height)   = = ~0<br> |
|  size\_t | [**m\_origin\_width**](#variable-m_origin_width)   = = ~0<br> |
|  size\_t | [**m\_pitch\_bytes**](#variable-m_pitch_bytes)   = = ~0<br> |
|  size\_t | [**m\_pitch\_bytes\_area**](#variable-m_pitch_bytes_area)   = = ~0<br> |








































## Public Types Documentation




### typedef CViewer 

```C++
using muda::Buffer3DViewT< IsConst, T >::CViewer =  CDense3D<T>;
```




<hr>



### typedef ConstView 

```C++
using muda::Buffer3DViewT< IsConst, T >::ConstView =  Buffer3DViewT<true, T>;
```




<hr>



### typedef NonConstView 

```C++
using muda::Buffer3DViewT< IsConst, T >::NonConstView =  Buffer3DViewT<false, T>;
```




<hr>



### typedef OtherView 

```C++
using muda::Buffer3DViewT< IsConst, T >::OtherView =  Buffer3DViewT<!IsConst, T>;
```




<hr>



### typedef ThisView 

```C++
using muda::Buffer3DViewT< IsConst, T >::ThisView =  Buffer3DViewT<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::Buffer3DViewT< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::Buffer3DViewT< IsConst, T >::Viewer =  Dense3D<T>;
```




<hr>
## Public Functions Documentation




### function Buffer3DViewT [2/6]

```C++
MUDA_GENERIC muda::Buffer3DViewT::Buffer3DViewT () 
```




<hr>



### function Buffer3DViewT [3/6]

```C++
MUDA_GENERIC muda::Buffer3DViewT::Buffer3DViewT (
    const Buffer3DViewT &
) 
```




<hr>



### function Buffer3DViewT [4/6]

```C++
template<bool OtherIsConst>
MUDA_GENERIC muda::Buffer3DViewT::Buffer3DViewT (
    const Buffer3DViewT < OtherIsConst, T > & other
) 
```




<hr>



### function Buffer3DViewT [5/6]

```C++
MUDA_GENERIC muda::Buffer3DViewT::Buffer3DViewT (
    auto_const_t< T > * data,
    size_t pitch_bytes,
    size_t pitch_bytes_area,
    size_t origin_width,
    size_t origin_height,
    const Offset3D & offset,
    const Extent3D & extent
) 
```




<hr>



### function Buffer3DViewT [6/6]

```C++
MUDA_GENERIC muda::Buffer3DViewT::Buffer3DViewT (
    T * data,
    size_t pitch_bytes,
    size_t pitch_bytes_area,
    const Offset3D & offset,
    const Extent3D & extent
) 
```




<hr>



### function as\_const 

```C++
MUDA_GENERIC ConstView muda::Buffer3DViewT::as_const () const
```




<hr>



### function copy\_from [1/2]

```C++
MUDA_HOST void muda::Buffer3DViewT::copy_from (
    const Buffer3DViewT < true, T > & other
) const
```




<hr>



### function copy\_from [2/2]

```C++
MUDA_HOST void muda::Buffer3DViewT::copy_from (
    const T * host
) const
```




<hr>



### function copy\_to 

```C++
MUDA_HOST void muda::Buffer3DViewT::copy_to (
    T * host
) const
```




<hr>



### function cviewer 

```C++
MUDA_GENERIC CViewer muda::Buffer3DViewT::cviewer () const
```




<hr>



### function data [1/2]

```C++
MUDA_GENERIC auto_const_t< T > * muda::Buffer3DViewT::data (
    size_t x,
    size_t y,
    size_t z
) const
```




<hr>



### function data [2/2]

```C++
MUDA_GENERIC auto_const_t< T > * muda::Buffer3DViewT::data (
    size_t flatten_i
) const
```




<hr>



### function extent 

```C++
MUDA_GENERIC Extent3D muda::Buffer3DViewT::extent () const
```




<hr>



### function fill 

```C++
MUDA_HOST void muda::Buffer3DViewT::fill (
    const T & v
) const
```




<hr>



### function offset 

```C++
MUDA_GENERIC Offset3D muda::Buffer3DViewT::offset () const
```




<hr>



### function origin\_data 

```C++
MUDA_GENERIC auto_const_t< T > * muda::Buffer3DViewT::origin_data () const
```




<hr>



### function pitch\_bytes 

```C++
MUDA_GENERIC size_t muda::Buffer3DViewT::pitch_bytes () const
```




<hr>



### function pitch\_bytes\_area 

```C++
MUDA_GENERIC size_t muda::Buffer3DViewT::pitch_bytes_area () const
```




<hr>



### function subview 

```C++
MUDA_GENERIC ThisView muda::Buffer3DViewT::subview (
    Offset3D offset,
    Extent3D extent={}
) const
```




<hr>



### function total\_size 

```C++
MUDA_GENERIC size_t muda::Buffer3DViewT::total_size () const
```




<hr>



### function viewer 

```C++
MUDA_GENERIC ThisViewer muda::Buffer3DViewT::viewer () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::Buffer3DViewT< IsConst, T >::m_data;
```




<hr>



### variable m\_extent 

```C++
Extent3D muda::Buffer3DViewT< IsConst, T >::m_extent;
```




<hr>



### variable m\_offset 

```C++
Offset3D muda::Buffer3DViewT< IsConst, T >::m_offset;
```




<hr>



### variable m\_origin\_height 

```C++
size_t muda::Buffer3DViewT< IsConst, T >::m_origin_height;
```




<hr>



### variable m\_origin\_width 

```C++
size_t muda::Buffer3DViewT< IsConst, T >::m_origin_width;
```




<hr>



### variable m\_pitch\_bytes 

```C++
size_t muda::Buffer3DViewT< IsConst, T >::m_pitch_bytes;
```




<hr>



### variable m\_pitch\_bytes\_area 

```C++
size_t muda::Buffer3DViewT< IsConst, T >::m_pitch_bytes_area;
```




<hr>## Friends Documentation





### friend BufferInfoAccessor 

```C++
class muda::Buffer3DViewT::BufferInfoAccessor (
    details::buffer::BufferInfoAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/buffer_3d_view.h`

