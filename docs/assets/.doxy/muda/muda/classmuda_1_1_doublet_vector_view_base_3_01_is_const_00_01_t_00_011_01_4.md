

# Class muda::DoubletVectorViewBase&lt; IsConst, T, 1 &gt;

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DoubletVectorViewBase&lt; IsConst, T, 1 &gt;**](classmuda_1_1_doublet_vector_view_base_3_01_is_const_00_01_t_00_011_01_4.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)&lt; true, T, 1 &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**CDoubletVectorViewer**](classmuda_1_1_c_doublet_vector_viewer.md)&lt; T, 1 &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)&lt; false, T, 1 &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**DoubletVectorViewer**](classmuda_1_1_doublet_vector_viewer.md)&lt; T, 1 &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**DoubletVectorViewBase**](classmuda_1_1_doublet_vector_view_base.md)&lt; IsConst, T, 1 &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_c_doublet_vector_viewer_3_01_t_00_011_01_4.md), [**NonConstViewer**](classmuda_1_1_doublet_vector_viewer_3_01_t_00_011_01_4.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |


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
|  MUDA\_GENERIC | [**DoubletVectorViewBase**](#function-doubletvectorviewbase-23) (int total\_count, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, int subvector\_offset, int subvector\_extent, auto\_const\_t&lt; int &gt; \* indices, auto\_const\_t&lt; T &gt; \* values) <br> |
|  MUDA\_GENERIC | [**DoubletVectorViewBase**](#function-doubletvectorviewbase-33) (int total\_count, int total\_doublet\_count, auto\_const\_t&lt; int &gt; \* indices, auto\_const\_t&lt; T &gt; \* values) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_doublet_vector_view_base.md) | [**as\_const**](#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_c_doublet_vector_viewer_3_01_t_00_011_01_4.md) | [**cviewer**](#function-cviewer) () noexcept const<br> |
|  MUDA\_GENERIC int | [**doublet\_count**](#function-doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC int | [**extent**](#function-extent) () noexcept const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](#function-operator-constview) () noexcept const<br> |
|  MUDA\_GENERIC auto | [**subvector**](#function-subvector) (int offset, int extent) noexcept const<br> |
|  MUDA\_GENERIC int | [**subvector\_offset**](#function-subvector_offset) () noexcept const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-12) (int offset, int count) noexcept const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-22) (int offset) noexcept const<br> |
|  MUDA\_GENERIC int | [**total\_doublet\_count**](#function-total_doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC int | [**total\_extent**](#function-total_extent) () noexcept const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](#function-viewer) () noexcept<br> |








## Protected Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_doublet\_count**](#variable-m_doublet_count)   = = 0<br> |
|  int | [**m\_doublet\_index\_offset**](#variable-m_doublet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_indices**](#variable-m_indices)  <br> |
|  int | [**m\_subvector\_extent**](#variable-m_subvector_extent)   = = 0<br> |
|  int | [**m\_subvector\_offset**](#variable-m_subvector_offset)   = = 0<br> |
|  int | [**m\_total\_count**](#variable-m_total_count)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](#variable-m_total_doublet_count)   = = 0<br> |
|  auto\_const\_t&lt; T &gt; \* | [**m\_values**](#variable-m_values)  <br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::ConstView =  DoubletVectorViewBase<true, T, 1>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::ConstViewer =  CDoubletVectorViewer<T, 1>;
```




<hr>



### typedef NonConstView 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::NonConstView =  DoubletVectorViewBase<false, T, 1>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::NonConstViewer =  DoubletVectorViewer<T, 1>;
```




<hr>



### typedef ThisView 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::ThisView =  DoubletVectorViewBase<IsConst, T, 1>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>
## Public Functions Documentation




### function DoubletVectorViewBase [1/3]

```C++
MUDA_GENERIC muda::DoubletVectorViewBase< IsConst, T, 1 >::DoubletVectorViewBase () = default
```




<hr>



### function DoubletVectorViewBase [2/3]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewBase< IsConst, T, 1 >::DoubletVectorViewBase (
    int total_count,
    int doublet_index_offset,
    int doublet_count,
    int total_doublet_count,
    int subvector_offset,
    int subvector_extent,
    auto_const_t< int > * indices,
    auto_const_t< T > * values
) 
```




<hr>



### function DoubletVectorViewBase [3/3]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewBase< IsConst, T, 1 >::DoubletVectorViewBase (
    int total_count,
    int total_doublet_count,
    auto_const_t< int > * indices,
    auto_const_t< T > * values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstView muda::DoubletVectorViewBase< IsConst, T, 1 >::as_const () noexcept const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC ConstViewer muda::DoubletVectorViewBase< IsConst, T, 1 >::cviewer () noexcept const
```




<hr>



### function doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase< IsConst, T, 1 >::doublet_count () noexcept const
```




<hr>



### function extent 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase< IsConst, T, 1 >::extent () noexcept const
```




<hr>



### function operator ConstView 

```C++
inline MUDA_GENERIC muda::DoubletVectorViewBase< IsConst, T, 1 >::operator ConstView () noexcept const
```




<hr>



### function subvector 

```C++
inline MUDA_GENERIC auto muda::DoubletVectorViewBase< IsConst, T, 1 >::subvector (
    int offset,
    int extent
) noexcept const
```




<hr>



### function subvector\_offset 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase< IsConst, T, 1 >::subvector_offset () noexcept const
```




<hr>



### function subview [1/2]

```C++
inline MUDA_GENERIC auto muda::DoubletVectorViewBase< IsConst, T, 1 >::subview (
    int offset,
    int count
) noexcept const
```




<hr>



### function subview [2/2]

```C++
inline MUDA_GENERIC auto muda::DoubletVectorViewBase< IsConst, T, 1 >::subview (
    int offset
) noexcept const
```




<hr>



### function total\_doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase< IsConst, T, 1 >::total_doublet_count () noexcept const
```




<hr>



### function total\_extent 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewBase< IsConst, T, 1 >::total_extent () noexcept const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC ThisViewer muda::DoubletVectorViewBase< IsConst, T, 1 >::viewer () noexcept
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::DoubletVectorViewBase< IsConst, T, 1 >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_doublet\_count 

```C++
int muda::DoubletVectorViewBase< IsConst, T, 1 >::m_doublet_count;
```




<hr>



### variable m\_doublet\_index\_offset 

```C++
int muda::DoubletVectorViewBase< IsConst, T, 1 >::m_doublet_index_offset;
```




<hr>



### variable m\_indices 

```C++
auto_const_t<int>* muda::DoubletVectorViewBase< IsConst, T, 1 >::m_indices;
```




<hr>



### variable m\_subvector\_extent 

```C++
int muda::DoubletVectorViewBase< IsConst, T, 1 >::m_subvector_extent;
```




<hr>



### variable m\_subvector\_offset 

```C++
int muda::DoubletVectorViewBase< IsConst, T, 1 >::m_subvector_offset;
```




<hr>



### variable m\_total\_count 

```C++
int muda::DoubletVectorViewBase< IsConst, T, 1 >::m_total_count;
```




<hr>



### variable m\_total\_doublet\_count 

```C++
int muda::DoubletVectorViewBase< IsConst, T, 1 >::m_total_doublet_count;
```




<hr>



### variable m\_values 

```C++
auto_const_t<T>* muda::DoubletVectorViewBase< IsConst, T, 1 >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/doublet_vector_view.h`

