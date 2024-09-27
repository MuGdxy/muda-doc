

# Class muda::DenseVectorViewBase

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseVectorViewBase**](classmuda_1_1_dense_vector_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef BufferView&lt; T &gt; | [**BufferView**](#typedef-bufferview)  <br> |
| typedef CBufferView&lt; T &gt; | [**CBufferView**](#typedef-cbufferview)  <br> |
| typedef [**CDenseVectorViewer**](classmuda_1_1_c_dense_vector_viewer.md)&lt; T &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**DenseVectorViewBase**](classmuda_1_1_dense_vector_view_base.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**DenseVectorViewBase**](classmuda_1_1_dense_vector_view_base.md)&lt; false, T &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBufferView, BufferView &gt; | [**ThisBufferView**](#typedef-thisbufferview)  <br> |
| typedef [**DenseVectorViewBase**](classmuda_1_1_dense_vector_view_base.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_c_dense_vector_viewer.md), [**Viewer**](classmuda_1_1_dense_vector_viewer.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**DenseVectorViewer**](classmuda_1_1_dense_vector_viewer.md)&lt; T &gt; | [**Viewer**](#typedef-viewer)  <br> |


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
|   | [**DenseVectorViewBase**](#function-densevectorviewbase-12) () = default<br> |
|   | [**DenseVectorViewBase**](#function-densevectorviewbase-22) (auto\_const\_t&lt; T &gt; \* data, cusparseDnVecDescr\_t descr, int offset, int inc, int size, int origin\_size) <br> |
|  [**ConstView**](classmuda_1_1_dense_vector_view_base.md) | [**as\_const**](#function-as_const) () const<br> |
|  auto | [**buffer\_view**](#function-buffer_view-12) () <br> |
|  CBufferView | [**buffer\_view**](#function-buffer_view-22) () const<br> |
|  auto | [**cviewer**](#function-cviewer) () const<br> |
|  auto | [**data**](#function-data-12) () <br> |
|  auto | [**data**](#function-data-22) () const<br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**inc**](#function-inc) () const<br> |
|  auto | [**offset**](#function-offset) () const<br> |
|   | [**operator ConstView**](#function-operator-constview) () const<br> |
|  auto | [**origin\_data**](#function-origin_data-12) () <br> |
|  auto | [**origin\_data**](#function-origin_data-22) () const<br> |
|  auto | [**size**](#function-size) () const<br> |
|  auto | [**subview**](#function-subview-12) (int offset, int size) <br> |
|  auto | [**subview**](#function-subview-22) (int offset, int size) const<br> |
|  auto | [**viewer**](#function-viewer) () <br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |
|  cusparseDnVecDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  int | [**m\_inc**](#variable-m_inc)   = = -1<br> |
|  int | [**m\_offset**](#variable-m_offset)   = = -1<br> |
|  int | [**m\_origin\_size**](#variable-m_origin_size)   = = -1<br> |
|  int | [**m\_size**](#variable-m_size)   = = -1<br> |








































## Public Types Documentation




### typedef BufferView 

```C++
using muda::DenseVectorViewBase< IsConst, T >::BufferView =  BufferView<T>;
```




<hr>



### typedef CBufferView 

```C++
using muda::DenseVectorViewBase< IsConst, T >::CBufferView =  CBufferView<T>;
```




<hr>



### typedef CViewer 

```C++
using muda::DenseVectorViewBase< IsConst, T >::CViewer =  CDenseVectorViewer<T>;
```




<hr>



### typedef ConstView 

```C++
using muda::DenseVectorViewBase< IsConst, T >::ConstView =  DenseVectorViewBase<true, T>;
```




<hr>



### typedef NonConstView 

```C++
using muda::DenseVectorViewBase< IsConst, T >::NonConstView =  DenseVectorViewBase<false, T>;
```




<hr>



### typedef ThisBufferView 

```C++
using muda::DenseVectorViewBase< IsConst, T >::ThisBufferView =  std::conditional_t<IsConst, CBufferView, BufferView>;
```




<hr>



### typedef ThisView 

```C++
using muda::DenseVectorViewBase< IsConst, T >::ThisView =  DenseVectorViewBase<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseVectorViewBase< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::DenseVectorViewBase< IsConst, T >::Viewer =  DenseVectorViewer<T>;
```




<hr>
## Public Functions Documentation




### function DenseVectorViewBase [1/2]

```C++
muda::DenseVectorViewBase::DenseVectorViewBase () = default
```




<hr>



### function DenseVectorViewBase [2/2]

```C++
inline muda::DenseVectorViewBase::DenseVectorViewBase (
    auto_const_t< T > * data,
    cusparseDnVecDescr_t descr,
    int offset,
    int inc,
    int size,
    int origin_size
) 
```




<hr>



### function as\_const 

```C++
inline ConstView muda::DenseVectorViewBase::as_const () const
```




<hr>



### function buffer\_view [1/2]

```C++
inline auto muda::DenseVectorViewBase::buffer_view () 
```




<hr>



### function buffer\_view [2/2]

```C++
inline CBufferView muda::DenseVectorViewBase::buffer_view () const
```




<hr>



### function cviewer 

```C++
inline auto muda::DenseVectorViewBase::cviewer () const
```




<hr>



### function data [1/2]

```C++
inline auto muda::DenseVectorViewBase::data () 
```




<hr>



### function data [2/2]

```C++
inline auto muda::DenseVectorViewBase::data () const
```




<hr>



### function descr 

```C++
inline auto muda::DenseVectorViewBase::descr () const
```




<hr>



### function inc 

```C++
inline auto muda::DenseVectorViewBase::inc () const
```




<hr>



### function offset 

```C++
inline auto muda::DenseVectorViewBase::offset () const
```




<hr>



### function operator ConstView 

```C++
inline muda::DenseVectorViewBase::operator ConstView () const
```




<hr>



### function origin\_data [1/2]

```C++
inline auto muda::DenseVectorViewBase::origin_data () 
```




<hr>



### function origin\_data [2/2]

```C++
inline auto muda::DenseVectorViewBase::origin_data () const
```




<hr>



### function size 

```C++
inline auto muda::DenseVectorViewBase::size () const
```




<hr>



### function subview [1/2]

```C++
inline auto muda::DenseVectorViewBase::subview (
    int offset,
    int size
) 
```




<hr>



### function subview [2/2]

```C++
inline auto muda::DenseVectorViewBase::subview (
    int offset,
    int size
) const
```




<hr>



### function viewer 

```C++
inline auto muda::DenseVectorViewBase::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::DenseVectorViewBase< IsConst, T >::m_data;
```




<hr>



### variable m\_descr 

```C++
cusparseDnVecDescr_t muda::DenseVectorViewBase< IsConst, T >::m_descr;
```




<hr>



### variable m\_inc 

```C++
int muda::DenseVectorViewBase< IsConst, T >::m_inc;
```




<hr>



### variable m\_offset 

```C++
int muda::DenseVectorViewBase< IsConst, T >::m_offset;
```




<hr>



### variable m\_origin\_size 

```C++
int muda::DenseVectorViewBase< IsConst, T >::m_origin_size;
```




<hr>



### variable m\_size 

```C++
int muda::DenseVectorViewBase< IsConst, T >::m_size;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_vector_view.h`

