

# Class muda::BufferViewT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**BufferViewT**](classmuda_1_1_buffer_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**CDense1D**](classmuda_1_1_dense1_d_t.md)&lt; T &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**BufferViewT**](classmuda_1_1_buffer_view_t.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**BufferViewT**](classmuda_1_1_buffer_view_t.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_dense1_d_t.md), [**Viewer**](classmuda_1_1_dense1_d_t.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**Dense1D**](classmuda_1_1_dense1_d_t.md)&lt; T &gt; | [**Viewer**](#typedef-viewer)  <br> |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |
| typedef size\_t | [**difference\_type**](#typedef-difference_type)  <br> |
| typedef std::random\_access\_iterator\_tag | [**iterator\_category**](#typedef-iterator_category)  <br> |
| typedef T \* | [**pointer**](#typedef-pointer)  <br> |
| typedef T & | [**reference**](#typedef-reference)  <br> |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |


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
|  MUDA\_GENERIC | [**BufferViewT**](#function-bufferviewt-26) () <br> |
|  MUDA\_GENERIC | [**BufferViewT**](#function-bufferviewt-36) (const [**BufferViewT**](classmuda_1_1_buffer_view_t.md) & other) <br> |
|  MUDA\_GENERIC | [**BufferViewT**](#function-bufferviewt-46) (auto\_const\_t&lt; T &gt; \* data, size\_t offset, size\_t size) <br> |
|  MUDA\_GENERIC | [**BufferViewT**](#function-bufferviewt-56) (auto\_const\_t&lt; T &gt; \* data, size\_t size) <br> |
|  MUDA\_GENERIC | [**BufferViewT**](#function-bufferviewt-66) (const [**BufferViewT**](classmuda_1_1_buffer_view_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_buffer_view_t.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-12) (const [**BufferViewT**](classmuda_1_1_buffer_view_t.md)&lt; true, T &gt; & other) const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-22) (const T \* host) const<br> |
|  MUDA\_HOST void | [**copy\_to**](#function-copy_to) (T \* host) const<br> |
|  MUDA\_GENERIC [**CViewer**](classmuda_1_1_dense1_d_t.md) | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-12) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-22) (size\_t i) const<br> |
|  MUDA\_HOST void | [**fill**](#function-fill) (const T & value) const<br> |
|  MUDA\_GENERIC size\_t | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC reference | [**operator\***](#function-operator) () const<br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_buffer_view_t.md) | [**operator+**](#function-operator_1) (int i) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator[]**](#function-operator_2) (size\_t i) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator[]**](#function-operator_3) (int i) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**origin\_data**](#function-origin_data) () const<br> |
|  MUDA\_GENERIC size\_t | [**size**](#function-size) () const<br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_buffer_view_t.md) | [**subview**](#function-subview) (size\_t offset, size\_t size=~0) const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](#function-viewer) () const<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |
|  size\_t | [**m\_offset**](#variable-m_offset)   = = ~0<br> |
|  size\_t | [**m\_size**](#variable-m_size)   = = ~0<br> |








































## Public Types Documentation




### typedef CViewer 

```C++
using muda::BufferViewT< IsConst, T >::CViewer =  CDense1D<T>;
```




<hr>



### typedef ConstView 

```C++
using muda::BufferViewT< IsConst, T >::ConstView =  BufferViewT<true, T>;
```




<hr>



### typedef ThisView 

```C++
using muda::BufferViewT< IsConst, T >::ThisView =  BufferViewT<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::BufferViewT< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::BufferViewT< IsConst, T >::Viewer =  Dense1D<T>;
```




<hr>



### typedef auto\_const\_t 

```C++
using muda::BufferViewT< IsConst, T >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>



### typedef difference\_type 

```C++
using muda::BufferViewT< IsConst, T >::difference_type =  size_t;
```




<hr>



### typedef iterator\_category 

```C++
using muda::BufferViewT< IsConst, T >::iterator_category =  std::random_access_iterator_tag;
```




<hr>



### typedef pointer 

```C++
using muda::BufferViewT< IsConst, T >::pointer =  T*;
```




<hr>



### typedef reference 

```C++
using muda::BufferViewT< IsConst, T >::reference =  T&;
```




<hr>



### typedef value\_type 

```C++
using muda::BufferViewT< IsConst, T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function BufferViewT [2/6]

```C++
MUDA_GENERIC muda::BufferViewT::BufferViewT () 
```




<hr>



### function BufferViewT [3/6]

```C++
MUDA_GENERIC muda::BufferViewT::BufferViewT (
    const BufferViewT & other
) 
```




<hr>



### function BufferViewT [4/6]

```C++
MUDA_GENERIC muda::BufferViewT::BufferViewT (
    auto_const_t< T > * data,
    size_t offset,
    size_t size
) 
```




<hr>



### function BufferViewT [5/6]

```C++
MUDA_GENERIC muda::BufferViewT::BufferViewT (
    auto_const_t< T > * data,
    size_t size
) 
```




<hr>



### function BufferViewT [6/6]

```C++
template<bool OtherIsConst>
MUDA_GENERIC muda::BufferViewT::BufferViewT (
    const BufferViewT < OtherIsConst, T > & other
) 
```




<hr>



### function as\_const 

```C++
MUDA_GENERIC ConstView muda::BufferViewT::as_const () const
```




<hr>



### function copy\_from [1/2]

```C++
MUDA_HOST void muda::BufferViewT::copy_from (
    const BufferViewT < true, T > & other
) const
```




<hr>



### function copy\_from [2/2]

```C++
MUDA_HOST void muda::BufferViewT::copy_from (
    const T * host
) const
```




<hr>



### function copy\_to 

```C++
MUDA_HOST void muda::BufferViewT::copy_to (
    T * host
) const
```




<hr>



### function cviewer 

```C++
MUDA_GENERIC CViewer muda::BufferViewT::cviewer () const
```




<hr>



### function data [1/2]

```C++
MUDA_GENERIC auto_const_t< T > * muda::BufferViewT::data () const
```




<hr>



### function data [2/2]

```C++
MUDA_GENERIC auto_const_t< T > * muda::BufferViewT::data (
    size_t i
) const
```




<hr>



### function fill 

```C++
MUDA_HOST void muda::BufferViewT::fill (
    const T & value
) const
```




<hr>



### function offset 

```C++
inline MUDA_GENERIC size_t muda::BufferViewT::offset () const
```




<hr>



### function operator\* 

```C++
MUDA_GENERIC reference muda::BufferViewT::operator* () const
```




<hr>



### function operator+ 

```C++
MUDA_GENERIC ThisView muda::BufferViewT::operator+ (
    int i
) const
```




<hr>



### function operator[] 

```C++
MUDA_GENERIC auto_const_t< T > & muda::BufferViewT::operator[] (
    size_t i
) const
```




<hr>



### function operator[] 

```C++
MUDA_GENERIC auto_const_t< T > & muda::BufferViewT::operator[] (
    int i
) const
```




<hr>



### function origin\_data 

```C++
MUDA_GENERIC auto_const_t< T > * muda::BufferViewT::origin_data () const
```




<hr>



### function size 

```C++
inline MUDA_GENERIC size_t muda::BufferViewT::size () const
```




<hr>



### function subview 

```C++
MUDA_GENERIC ThisView muda::BufferViewT::subview (
    size_t offset,
    size_t size=~0
) const
```




<hr>



### function viewer 

```C++
MUDA_GENERIC ThisViewer muda::BufferViewT::viewer () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::BufferViewT< IsConst, T >::m_data;
```




<hr>



### variable m\_offset 

```C++
size_t muda::BufferViewT< IsConst, T >::m_offset;
```




<hr>



### variable m\_size 

```C++
size_t muda::BufferViewT< IsConst, T >::m_size;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/buffer_fwd.h`

