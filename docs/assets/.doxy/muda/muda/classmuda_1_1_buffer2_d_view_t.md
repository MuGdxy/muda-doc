

# Class muda::Buffer2DViewT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Buffer2DViewT**](classmuda_1_1_buffer2_d_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**CDense2D**](classmuda_1_1_dense2_d_base.md)&lt; T &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**Buffer2DViewT**](classmuda_1_1_buffer2_d_view_t.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**Buffer2DViewT**](classmuda_1_1_buffer2_d_view_t.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_dense2_d_base.md), [**Viewer**](classmuda_1_1_dense2_d_base.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**Dense2D**](classmuda_1_1_dense2_d_base.md)&lt; T &gt; | [**Viewer**](#typedef-viewer)  <br> |


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
|  MUDA\_GENERIC | [**Buffer2DViewT**](#function-buffer2dviewt-26) () <br> |
|  MUDA\_GENERIC | [**Buffer2DViewT**](#function-buffer2dviewt-36) (const [**Buffer2DViewT**](classmuda_1_1_buffer2_d_view_t.md) &) <br> |
|  MUDA\_GENERIC | [**Buffer2DViewT**](#function-buffer2dviewt-46) (const [**Buffer2DViewT**](classmuda_1_1_buffer2_d_view_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC | [**Buffer2DViewT**](#function-buffer2dviewt-56) (auto\_const\_t&lt; T &gt; \* data, size\_t pitch\_bytes, size\_t origin\_width, size\_t origin\_height, const [**Offset2D**](classmuda_1_1_offset2_d.md) & offset, const [**Extent2D**](classmuda_1_1_extent2_d.md) & extent) <br> |
|  MUDA\_GENERIC | [**Buffer2DViewT**](#function-buffer2dviewt-66) (auto\_const\_t&lt; T &gt; \* data, size\_t pitch\_bytes, const [**Offset2D**](classmuda_1_1_offset2_d.md) & offset, const [**Extent2D**](classmuda_1_1_extent2_d.md) & extent) <br> |
|  [**ConstView**](classmuda_1_1_buffer2_d_view_t.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-12) (const [**Buffer2DViewT**](classmuda_1_1_buffer2_d_view_t.md)&lt; true, T &gt; & other) <br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-22) (const T \* host) <br> |
|  MUDA\_HOST void | [**copy\_to**](#function-copy_to) (T \* host) const<br> |
|  MUDA\_GENERIC [**CViewer**](classmuda_1_1_dense2_d_base.md) | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-12) (size\_t x, size\_t y) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-22) (size\_t flatten\_i) const<br> |
|  MUDA\_GENERIC [**Extent2D**](classmuda_1_1_extent2_d.md) | [**extent**](#function-extent) () const<br> |
|  MUDA\_HOST void | [**fill**](#function-fill) (const T & v) <br> |
|  MUDA\_GENERIC [**Offset2D**](classmuda_1_1_offset2_d.md) | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**origin\_data**](#function-origin_data) () const<br> |
|  MUDA\_GENERIC size\_t | [**pitch\_bytes**](#function-pitch_bytes) () const<br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_buffer2_d_view_t.md) | [**subview**](#function-subview) ([**Offset2D**](classmuda_1_1_offset2_d.md) offset, [**Extent2D**](classmuda_1_1_extent2_d.md) extent={}) const<br> |
|  MUDA\_GENERIC size\_t | [**total\_size**](#function-total_size) () const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](#function-viewer) () const<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |
|  [**Extent2D**](classmuda_1_1_extent2_d.md) | [**m\_extent**](#variable-m_extent)  <br> |
|  [**Offset2D**](classmuda_1_1_offset2_d.md) | [**m\_offset**](#variable-m_offset)  <br> |
|  size\_t | [**m\_origin\_height**](#variable-m_origin_height)   = = 0<br> |
|  size\_t | [**m\_origin\_width**](#variable-m_origin_width)   = = 0<br> |
|  size\_t | [**m\_pitch\_bytes**](#variable-m_pitch_bytes)   = = ~0<br> |








































## Public Types Documentation




### typedef CViewer 

```C++
using muda::Buffer2DViewT< IsConst, T >::CViewer =  CDense2D<T>;
```




<hr>



### typedef ConstView 

```C++
using muda::Buffer2DViewT< IsConst, T >::ConstView =  Buffer2DViewT<true, T>;
```




<hr>



### typedef ThisView 

```C++
using muda::Buffer2DViewT< IsConst, T >::ThisView =  Buffer2DViewT<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::Buffer2DViewT< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::Buffer2DViewT< IsConst, T >::Viewer =  Dense2D<T>;
```




<hr>
## Public Functions Documentation




### function Buffer2DViewT [2/6]

```C++
MUDA_GENERIC muda::Buffer2DViewT::Buffer2DViewT () 
```




<hr>



### function Buffer2DViewT [3/6]

```C++
MUDA_GENERIC muda::Buffer2DViewT::Buffer2DViewT (
    const Buffer2DViewT &
) 
```




<hr>



### function Buffer2DViewT [4/6]

```C++
template<bool OtherIsConst>
MUDA_GENERIC muda::Buffer2DViewT::Buffer2DViewT (
    const Buffer2DViewT < OtherIsConst, T > & other
) 
```




<hr>



### function Buffer2DViewT [5/6]

```C++
MUDA_GENERIC muda::Buffer2DViewT::Buffer2DViewT (
    auto_const_t< T > * data,
    size_t pitch_bytes,
    size_t origin_width,
    size_t origin_height,
    const Offset2D & offset,
    const Extent2D & extent
) 
```




<hr>



### function Buffer2DViewT [6/6]

```C++
MUDA_GENERIC muda::Buffer2DViewT::Buffer2DViewT (
    auto_const_t< T > * data,
    size_t pitch_bytes,
    const Offset2D & offset,
    const Extent2D & extent
) 
```




<hr>



### function as\_const 

```C++
ConstView muda::Buffer2DViewT::as_const () const
```




<hr>



### function copy\_from [1/2]

```C++
MUDA_HOST void muda::Buffer2DViewT::copy_from (
    const Buffer2DViewT < true, T > & other
) 
```




<hr>



### function copy\_from [2/2]

```C++
MUDA_HOST void muda::Buffer2DViewT::copy_from (
    const T * host
) 
```




<hr>



### function copy\_to 

```C++
MUDA_HOST void muda::Buffer2DViewT::copy_to (
    T * host
) const
```




<hr>



### function cviewer 

```C++
MUDA_GENERIC CViewer muda::Buffer2DViewT::cviewer () const
```




<hr>



### function data [1/2]

```C++
MUDA_GENERIC auto_const_t< T > * muda::Buffer2DViewT::data (
    size_t x,
    size_t y
) const
```




<hr>



### function data [2/2]

```C++
MUDA_GENERIC auto_const_t< T > * muda::Buffer2DViewT::data (
    size_t flatten_i
) const
```




<hr>



### function extent 

```C++
MUDA_GENERIC Extent2D muda::Buffer2DViewT::extent () const
```




<hr>



### function fill 

```C++
MUDA_HOST void muda::Buffer2DViewT::fill (
    const T & v
) 
```




<hr>



### function offset 

```C++
MUDA_GENERIC Offset2D muda::Buffer2DViewT::offset () const
```




<hr>



### function origin\_data 

```C++
MUDA_GENERIC auto_const_t< T > * muda::Buffer2DViewT::origin_data () const
```




<hr>



### function pitch\_bytes 

```C++
MUDA_GENERIC size_t muda::Buffer2DViewT::pitch_bytes () const
```




<hr>



### function subview 

```C++
MUDA_GENERIC ThisView muda::Buffer2DViewT::subview (
    Offset2D offset,
    Extent2D extent={}
) const
```




<hr>



### function total\_size 

```C++
MUDA_GENERIC size_t muda::Buffer2DViewT::total_size () const
```




<hr>



### function viewer 

```C++
MUDA_GENERIC ThisViewer muda::Buffer2DViewT::viewer () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::Buffer2DViewT< IsConst, T >::m_data;
```




<hr>



### variable m\_extent 

```C++
Extent2D muda::Buffer2DViewT< IsConst, T >::m_extent;
```




<hr>



### variable m\_offset 

```C++
Offset2D muda::Buffer2DViewT< IsConst, T >::m_offset;
```




<hr>



### variable m\_origin\_height 

```C++
size_t muda::Buffer2DViewT< IsConst, T >::m_origin_height;
```




<hr>



### variable m\_origin\_width 

```C++
size_t muda::Buffer2DViewT< IsConst, T >::m_origin_width;
```




<hr>



### variable m\_pitch\_bytes 

```C++
size_t muda::Buffer2DViewT< IsConst, T >::m_pitch_bytes;
```




<hr>## Friends Documentation





### friend BufferInfoAccessor 

```C++
class muda::Buffer2DViewT::BufferInfoAccessor (
    details::buffer::BufferInfoAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/buffer_2d_view.h`

