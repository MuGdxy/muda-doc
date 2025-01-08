

# Class muda::DenseVectorViewT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseVectorViewT**](classmuda_1_1_dense_vector_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef BufferView&lt; T &gt; | [**BufferView**](#typedef-bufferview)  <br> |
| typedef CBufferView&lt; T &gt; | [**CBufferView**](#typedef-cbufferview)  <br> |
| typedef [**CDenseVectorViewer**](classmuda_1_1_dense_vector_viewer_t.md)&lt; T &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**DenseVectorViewT**](classmuda_1_1_dense_vector_view_t.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**DenseVectorViewT**](classmuda_1_1_dense_vector_view_t.md)&lt; false, T &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBufferView, BufferView &gt; | [**ThisBufferView**](#typedef-thisbufferview)  <br> |
| typedef [**DenseVectorViewT**](classmuda_1_1_dense_vector_view_t.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_dense_vector_viewer_t.md), [**Viewer**](classmuda_1_1_dense_vector_viewer_t.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**DenseVectorViewer**](classmuda_1_1_dense_vector_viewer_t.md)&lt; T &gt; | [**Viewer**](#typedef-viewer)  <br> |


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
|  MUDA\_GENERIC | [**DenseVectorViewT**](#function-densevectorviewt-24) () = default<br> |
|  MUDA\_GENERIC | [**DenseVectorViewT**](#function-densevectorviewt-34) (auto\_const\_t&lt; T &gt; \* data, cusparseDnVecDescr\_t descr, int offset, int inc, int size, int origin\_size) <br> |
|  MUDA\_GENERIC | [**DenseVectorViewT**](#function-densevectorviewt-44) (const [**DenseVectorViewT**](classmuda_1_1_dense_vector_view_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_dense_vector_view_t.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](#function-buffer_view) () const<br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto | [**data**](#function-data) () const<br> |
|  MUDA\_GENERIC auto | [**descr**](#function-descr) () const<br> |
|  MUDA\_GENERIC auto | [**inc**](#function-inc) () const<br> |
|  MUDA\_GENERIC auto | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC auto | [**origin\_data**](#function-origin_data) () const<br> |
|  MUDA\_GENERIC auto | [**size**](#function-size) () const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview) (int offset, int size) const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () const<br> |
















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
using muda::DenseVectorViewT< IsConst, T >::BufferView =  BufferView<T>;
```




<hr>



### typedef CBufferView 

```C++
using muda::DenseVectorViewT< IsConst, T >::CBufferView =  CBufferView<T>;
```




<hr>



### typedef CViewer 

```C++
using muda::DenseVectorViewT< IsConst, T >::CViewer =  CDenseVectorViewer<T>;
```




<hr>



### typedef ConstView 

```C++
using muda::DenseVectorViewT< IsConst, T >::ConstView =  DenseVectorViewT<true, T>;
```




<hr>



### typedef NonConstView 

```C++
using muda::DenseVectorViewT< IsConst, T >::NonConstView =  DenseVectorViewT<false, T>;
```




<hr>



### typedef ThisBufferView 

```C++
using muda::DenseVectorViewT< IsConst, T >::ThisBufferView =  std::conditional_t<IsConst, CBufferView, BufferView>;
```




<hr>



### typedef ThisView 

```C++
using muda::DenseVectorViewT< IsConst, T >::ThisView =  DenseVectorViewT<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseVectorViewT< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::DenseVectorViewT< IsConst, T >::Viewer =  DenseVectorViewer<T>;
```




<hr>
## Public Functions Documentation




### function DenseVectorViewT [2/4]

```C++
MUDA_GENERIC muda::DenseVectorViewT::DenseVectorViewT () = default
```




<hr>



### function DenseVectorViewT [3/4]

```C++
inline MUDA_GENERIC muda::DenseVectorViewT::DenseVectorViewT (
    auto_const_t< T > * data,
    cusparseDnVecDescr_t descr,
    int offset,
    int inc,
    int size,
    int origin_size
) 
```




<hr>



### function DenseVectorViewT [4/4]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::DenseVectorViewT::DenseVectorViewT (
    const DenseVectorViewT < OtherIsConst, T > & other
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstView muda::DenseVectorViewT::as_const () const
```




<hr>



### function buffer\_view 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::buffer_view () const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::cviewer () const
```




<hr>



### function data 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::data () const
```




<hr>



### function descr 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::descr () const
```




<hr>



### function inc 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::inc () const
```




<hr>



### function offset 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::offset () const
```




<hr>



### function origin\_data 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::origin_data () const
```




<hr>



### function size 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::size () const
```




<hr>



### function subview 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::subview (
    int offset,
    int size
) const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewT::viewer () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::DenseVectorViewT< IsConst, T >::m_data;
```




<hr>



### variable m\_descr 

```C++
cusparseDnVecDescr_t muda::DenseVectorViewT< IsConst, T >::m_descr;
```




<hr>



### variable m\_inc 

```C++
int muda::DenseVectorViewT< IsConst, T >::m_inc;
```




<hr>



### variable m\_offset 

```C++
int muda::DenseVectorViewT< IsConst, T >::m_offset;
```




<hr>



### variable m\_origin\_size 

```C++
int muda::DenseVectorViewT< IsConst, T >::m_origin_size;
```




<hr>



### variable m\_size 

```C++
int muda::DenseVectorViewT< IsConst, T >::m_size;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_vector_view.h`

