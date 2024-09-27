

# Class muda::COOVectorViewBase

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**COOVectorViewBase**](classmuda_1_1_c_o_o_vector_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**CCOOVectorViewer**](classmuda_1_1_c_doublet_vector_viewer.md)&lt; T &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**COOVectorViewBase**](classmuda_1_1_c_o_o_vector_view_base.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**COOVectorViewBase**](classmuda_1_1_c_o_o_vector_view_base.md)&lt; false, T &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**COOVectorViewBase**](classmuda_1_1_c_o_o_vector_view_base.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_c_doublet_vector_viewer.md), [**Viewer**](classmuda_1_1_c_doublet_vector_viewer.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**COOVectorViewer**](classmuda_1_1_c_doublet_vector_viewer.md)&lt; T &gt; | [**Viewer**](#typedef-viewer)  <br> |


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
|  MUDA\_GENERIC | [**COOVectorViewBase**](#function-coovectorviewbase-12) () = default<br> |
|  MUDA\_GENERIC | [**COOVectorViewBase**](#function-coovectorviewbase-22) (int size, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, auto\_const\_t&lt; int &gt; \* indices, auto\_const\_t&lt; T &gt; \* values, cusparseSpVecDescr\_t descr) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto | [**descr**](#function-descr) () const<br> |
|  MUDA\_GENERIC auto | [**doublet\_count**](#function-doublet_count) () const<br> |
|  MUDA\_GENERIC auto | [**doublet\_index\_offset**](#function-doublet_index_offset) () const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](#function-operator-constview) () const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-14) (int offset, int count) <br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-24) (int offset) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_c_o_o_vector_view_base.md) | [**subview**](#function-subview-34) (int offset, int count) const<br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_c_o_o_vector_view_base.md) | [**subview**](#function-subview-44) (int offset) const<br> |
|  MUDA\_GENERIC auto | [**total\_doublet\_count**](#function-total_doublet_count) () const<br> |
|  MUDA\_GENERIC auto | [**vector\_size**](#function-vector_size) () const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () <br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  cusparseSpVecDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  int | [**m\_doublet\_count**](#variable-m_doublet_count)   = = 0<br> |
|  int | [**m\_doublet\_index\_offset**](#variable-m_doublet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_indices**](#variable-m_indices)   = = nullptr<br> |
|  int | [**m\_size**](#variable-m_size)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](#variable-m_total_doublet_count)   = = 0<br> |
|  auto\_const\_t&lt; T &gt; \* | [**m\_values**](#variable-m_values)   = = nullptr<br> |








































## Public Types Documentation




### typedef CViewer 

```C++
using muda::COOVectorViewBase< IsConst, T >::CViewer =  CCOOVectorViewer<T>;
```




<hr>



### typedef ConstView 

```C++
using muda::COOVectorViewBase< IsConst, T >::ConstView =  COOVectorViewBase<true, T>;
```




<hr>



### typedef NonConstView 

```C++
using muda::COOVectorViewBase< IsConst, T >::NonConstView =  COOVectorViewBase<false, T>;
```




<hr>



### typedef ThisView 

```C++
using muda::COOVectorViewBase< IsConst, T >::ThisView =  COOVectorViewBase<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::COOVectorViewBase< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::COOVectorViewBase< IsConst, T >::Viewer =  COOVectorViewer<T>;
```




<hr>
## Public Functions Documentation




### function COOVectorViewBase [1/2]

```C++
MUDA_GENERIC muda::COOVectorViewBase::COOVectorViewBase () = default
```




<hr>



### function COOVectorViewBase [2/2]

```C++
inline MUDA_GENERIC muda::COOVectorViewBase::COOVectorViewBase (
    int size,
    int doublet_index_offset,
    int doublet_count,
    int total_doublet_count,
    auto_const_t< int > * indices,
    auto_const_t< T > * values,
    cusparseSpVecDescr_t descr
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::as_const () const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::cviewer () const
```




<hr>



### function descr 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::descr () const
```




<hr>



### function doublet\_count 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::doublet_count () const
```




<hr>



### function doublet\_index\_offset 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::doublet_index_offset () const
```




<hr>



### function operator ConstView 

```C++
inline MUDA_GENERIC muda::COOVectorViewBase::operator ConstView () const
```




<hr>



### function subview [1/4]

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::subview (
    int offset,
    int count
) 
```




<hr>



### function subview [2/4]

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::subview (
    int offset
) 
```




<hr>



### function subview [3/4]

```C++
inline MUDA_GENERIC ConstView muda::COOVectorViewBase::subview (
    int offset,
    int count
) const
```




<hr>



### function subview [4/4]

```C++
inline MUDA_GENERIC ConstView muda::COOVectorViewBase::subview (
    int offset
) const
```




<hr>



### function total\_doublet\_count 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::total_doublet_count () const
```




<hr>



### function vector\_size 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::vector_size () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::COOVectorViewBase::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_descr 

```C++
cusparseSpVecDescr_t muda::COOVectorViewBase< IsConst, T >::m_descr;
```




<hr>



### variable m\_doublet\_count 

```C++
int muda::COOVectorViewBase< IsConst, T >::m_doublet_count;
```




<hr>



### variable m\_doublet\_index\_offset 

```C++
int muda::COOVectorViewBase< IsConst, T >::m_doublet_index_offset;
```




<hr>



### variable m\_indices 

```C++
auto_const_t<int>* muda::COOVectorViewBase< IsConst, T >::m_indices;
```




<hr>



### variable m\_size 

```C++
int muda::COOVectorViewBase< IsConst, T >::m_size;
```




<hr>



### variable m\_total\_doublet\_count 

```C++
int muda::COOVectorViewBase< IsConst, T >::m_total_doublet_count;
```




<hr>



### variable m\_values 

```C++
auto_const_t<T>* muda::COOVectorViewBase< IsConst, T >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/bcoo_vector_view.h`

