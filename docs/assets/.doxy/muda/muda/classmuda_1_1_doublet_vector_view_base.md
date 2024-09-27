

# Class muda::DoubletVectorViewBase

**template &lt;bool IsConst, typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)&lt; true, T, N &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**CDoubletVectorViewer**](classmuda_1_1_c_doublet_vector_viewer.md)&lt; T, N &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)&lt; false, T, N &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**DoubletVectorViewer**](classmuda_1_1_doublet_vector_viewer.md)&lt; T, N &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef Eigen::Matrix&lt; T, N, 1 &gt; | [**SegmentVector**](#typedef-segmentvector)  <br> |
| typedef [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)&lt; IsConst, T, N &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_c_doublet_vector_viewer.md), [**NonConstViewer**](classmuda_1_1_doublet_vector_viewer.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |


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
|  MUDA\_GENERIC | [**DoubletVectorViewBase**](#function-doubletvectorviewbase-13) () = default<br> |
|  MUDA\_GENERIC | [**DoubletVectorViewBase**](#function-doubletvectorviewbase-23) (int total\_segment\_count, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, int subvector\_offset, int subvector\_extent, auto\_const\_t&lt; int &gt; \* segment\_indices, auto\_const\_t&lt; SegmentVector &gt; \* segment\_values) <br> |
|  MUDA\_GENERIC | [**DoubletVectorViewBase**](#function-doubletvectorviewbase-33) (int total\_segment\_count, int total\_doublet\_count, auto\_const\_t&lt; int &gt; \* segment\_indices, auto\_const\_t&lt; SegmentVector &gt; \* segment\_values) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_doublet_vector_view_base.md) | [**as\_const**](#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_c_doublet_vector_viewer.md) | [**cviewer**](#function-cviewer) () noexcept const<br> |
|  MUDA\_GENERIC int | [**doublet\_count**](#function-doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC int | [**extent**](#function-extent) () noexcept const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](#function-operator-constview) () noexcept const<br> |
|  MUDA\_GENERIC auto | [**subvector**](#function-subvector) (int offset, int extent) noexcept const<br> |
|  MUDA\_GENERIC int | [**subvector\_offset**](#function-subvector_offset) () noexcept const<br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_doublet_vector_view_base.md) | [**subview**](#function-subview-12) (int offset, int count) noexcept const<br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_doublet_vector_view_base.md) | [**subview**](#function-subview-22) (int offset) noexcept const<br> |
|  MUDA\_GENERIC int | [**total\_doublet\_count**](#function-total_doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC int | [**total\_extent**](#function-total_extent) () noexcept const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](#function-viewer) () noexcept<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_doublet\_count**](#variable-m_doublet_count)   = = 0<br> |
|  int | [**m\_doublet\_index\_offset**](#variable-m_doublet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_segment\_indices**](#variable-m_segment_indices)  <br> |
|  auto\_const\_t&lt; SegmentVector &gt; \* | [**m\_segment\_values**](#variable-m_segment_values)  <br> |
|  int | [**m\_subvector\_extent**](#variable-m_subvector_extent)   = = 0<br> |
|  int | [**m\_subvector\_offset**](#variable-m_subvector_offset)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](#variable-m_total_doublet_count)   = = 0<br> |
|  int | [**m\_total\_segment\_count**](#variable-m_total_segment_count)   = = 0<br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::ConstView =  DoubletVectorViewBase<true, T, N>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::ConstViewer =  CDoubletVectorViewer<T, N>;
```




<hr>



### typedef NonConstView 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::NonConstView =  DoubletVectorViewBase<false, T, N>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::NonConstViewer =  DoubletVectorViewer<T, N>;
```




<hr>



### typedef SegmentVector 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::SegmentVector =  Eigen::Matrix<T, N, 1>;
```




<hr>



### typedef ThisView 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::ThisView =  DoubletVectorViewBase<IsConst, T, N>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DoubletVectorViewBase< IsConst, T, N >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>
## Public Functions Documentation




### function DoubletVectorViewBase [1/3]

```C++
MUDA_GENERIC muda::DoubletVectorViewBase::DoubletVectorViewBase () = default
```




<hr>



### function DoubletVectorViewBase [2/3]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewBase::DoubletVectorViewBase (
    int total_segment_count,
    int doublet_index_offset,
    int doublet_count,
    int total_doublet_count,
    int subvector_offset,
    int subvector_extent,
    auto_const_t< int > * segment_indices,
    auto_const_t< SegmentVector > * segment_values
) 
```




<hr>



### function DoubletVectorViewBase [3/3]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewBase::DoubletVectorViewBase (
    int total_segment_count,
    int total_doublet_count,
    auto_const_t< int > * segment_indices,
    auto_const_t< SegmentVector > * segment_values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstView muda::DoubletVectorViewBase::as_const () noexcept const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC ConstViewer muda::DoubletVectorViewBase::cviewer () noexcept const
```




<hr>



### function doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase::doublet_count () noexcept const
```




<hr>



### function extent 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase::extent () noexcept const
```




<hr>



### function operator ConstView 

```C++
inline MUDA_GENERIC muda::DoubletVectorViewBase::operator ConstView () noexcept const
```




<hr>



### function subvector 

```C++
inline MUDA_GENERIC auto muda::DoubletVectorViewBase::subvector (
    int offset,
    int extent
) noexcept const
```




<hr>



### function subvector\_offset 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase::subvector_offset () noexcept const
```




<hr>



### function subview [1/2]

```C++
inline MUDA_GENERIC ThisView muda::DoubletVectorViewBase::subview (
    int offset,
    int count
) noexcept const
```




<hr>



### function subview [2/2]

```C++
inline MUDA_GENERIC ThisView muda::DoubletVectorViewBase::subview (
    int offset
) noexcept const
```




<hr>



### function total\_doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase::total_doublet_count () noexcept const
```




<hr>



### function total\_extent 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase::total_extent () noexcept const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC ThisViewer muda::DoubletVectorViewBase::viewer () noexcept
```




<hr>
## Protected Attributes Documentation




### variable m\_doublet\_count 

```C++
int muda::DoubletVectorViewBase< IsConst, T, N >::m_doublet_count;
```




<hr>



### variable m\_doublet\_index\_offset 

```C++
int muda::DoubletVectorViewBase< IsConst, T, N >::m_doublet_index_offset;
```




<hr>



### variable m\_segment\_indices 

```C++
auto_const_t<int>* muda::DoubletVectorViewBase< IsConst, T, N >::m_segment_indices;
```




<hr>



### variable m\_segment\_values 

```C++
auto_const_t<SegmentVector>* muda::DoubletVectorViewBase< IsConst, T, N >::m_segment_values;
```




<hr>



### variable m\_subvector\_extent 

```C++
int muda::DoubletVectorViewBase< IsConst, T, N >::m_subvector_extent;
```




<hr>



### variable m\_subvector\_offset 

```C++
int muda::DoubletVectorViewBase< IsConst, T, N >::m_subvector_offset;
```




<hr>



### variable m\_total\_doublet\_count 

```C++
int muda::DoubletVectorViewBase< IsConst, T, N >::m_total_doublet_count;
```




<hr>



### variable m\_total\_segment\_count 

```C++
int muda::DoubletVectorViewBase< IsConst, T, N >::m_total_segment_count;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/doublet_vector_view.h`
