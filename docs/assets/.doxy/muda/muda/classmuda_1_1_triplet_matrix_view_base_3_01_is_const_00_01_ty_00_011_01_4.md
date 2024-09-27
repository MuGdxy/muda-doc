

# Class muda::TripletMatrixViewBase&lt; IsConst, Ty, 1 &gt;

**template &lt;bool IsConst, typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**TripletMatrixViewBase&lt; IsConst, Ty, 1 &gt;**](classmuda_1_1_triplet_matrix_view_base_3_01_is_const_00_01_ty_00_011_01_4.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)&lt; true, Ty, 1 &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)&lt; false, Ty, 1 &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)&lt; IsConst, Ty, 1 &gt; | [**ThisView**](#typedef-thisview)  <br> |


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
|  MUDA\_GENERIC | [**TripletMatrixViewBase**](#function-tripletmatrixviewbase-13) () = default<br> |
|  MUDA\_GENERIC | [**TripletMatrixViewBase**](#function-tripletmatrixviewbase-23) (int total\_rows, int total\_cols, int triplet\_index\_offset, int triplet\_count, int total\_triplet\_count, int2 submatrix\_offset, int2 submatrix\_extent, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values) <br> |
|  MUDA\_GENERIC | [**TripletMatrixViewBase**](#function-tripletmatrixviewbase-33) (int total\_rows, int total\_cols, int total\_triplet\_count, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_triplet_matrix_view_base.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; int &gt; \* | [**col\_indices**](#function-col_indices-12) () <br> |
|  MUDA\_GENERIC auto | [**col\_indices**](#function-col_indices-22) () const<br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto | [**extent**](#function-extent) () const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](#function-operator-constview) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; int &gt; \* | [**row\_indices**](#function-row_indices-12) () <br> |
|  MUDA\_GENERIC auto | [**row\_indices**](#function-row_indices-22) () const<br> |
|  MUDA\_GENERIC auto | [**submatrix**](#function-submatrix) (int2 offset, int2 extent) const<br> |
|  MUDA\_GENERIC auto | [**submatrix\_offset**](#function-submatrix_offset) () const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-12) (int offset, int count) const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-22) (int offset) const<br> |
|  MUDA\_GENERIC auto | [**total\_cols**](#function-total_cols) () const<br> |
|  MUDA\_GENERIC auto | [**total\_extent**](#function-total_extent) () const<br> |
|  MUDA\_GENERIC auto | [**total\_rows**](#function-total_rows) () const<br> |
|  MUDA\_GENERIC auto | [**total\_triplet\_count**](#function-total_triplet_count) () const<br> |
|  MUDA\_GENERIC auto | [**tripet\_index\_offset**](#function-tripet_index_offset) () const<br> |
|  MUDA\_GENERIC auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; Ty &gt; \* | [**values**](#function-values-12) () <br> |
|  MUDA\_GENERIC auto | [**values**](#function-values-22) () const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () <br> |








## Protected Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; int &gt; \* | [**m\_col\_indices**](#variable-m_col_indices)  <br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_row\_indices**](#variable-m_row_indices)  <br> |
|  int2 | [**m\_submatrix\_extent**](#variable-m_submatrix_extent)   = = {0, 0}<br> |
|  int2 | [**m\_submatrix\_offset**](#variable-m_submatrix_offset)   = = {0, 0}<br> |
|  int | [**m\_total\_cols**](#variable-m_total_cols)   = = 0<br> |
|  int | [**m\_total\_rows**](#variable-m_total_rows)   = = 0<br> |
|  int | [**m\_total\_triplet\_count**](#variable-m_total_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_count**](#variable-m_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_index\_offset**](#variable-m_triplet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; Ty &gt; \* | [**m\_values**](#variable-m_values)  <br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, 1 >::ConstView =  TripletMatrixViewBase<true, Ty, 1>;
```




<hr>



### typedef NonConstView 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, 1 >::NonConstView =  TripletMatrixViewBase<false, Ty, 1>;
```




<hr>



### typedef ThisView 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, 1 >::ThisView =  TripletMatrixViewBase<IsConst, Ty, 1>;
```




<hr>
## Public Functions Documentation




### function TripletMatrixViewBase [1/3]

```C++
MUDA_GENERIC muda::TripletMatrixViewBase< IsConst, Ty, 1 >::TripletMatrixViewBase () = default
```




<hr>



### function TripletMatrixViewBase [2/3]

```C++
inline MUDA_GENERIC muda::TripletMatrixViewBase< IsConst, Ty, 1 >::TripletMatrixViewBase (
    int total_rows,
    int total_cols,
    int triplet_index_offset,
    int triplet_count,
    int total_triplet_count,
    int2 submatrix_offset,
    int2 submatrix_extent,
    auto_const_t< int > * row_indices,
    auto_const_t< int > * col_indices,
    auto_const_t< Ty > * values
) 
```




<hr>



### function TripletMatrixViewBase [3/3]

```C++
inline MUDA_GENERIC muda::TripletMatrixViewBase< IsConst, Ty, 1 >::TripletMatrixViewBase (
    int total_rows,
    int total_cols,
    int total_triplet_count,
    auto_const_t< int > * row_indices,
    auto_const_t< int > * col_indices,
    auto_const_t< Ty > * values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstView muda::TripletMatrixViewBase< IsConst, Ty, 1 >::as_const () const
```




<hr>



### function col\_indices [1/2]

```C++
inline MUDA_GENERIC auto_const_t< int > * muda::TripletMatrixViewBase< IsConst, Ty, 1 >::col_indices () 
```




<hr>



### function col\_indices [2/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::col_indices () const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::cviewer () const
```




<hr>



### function extent 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::extent () const
```




<hr>



### function operator ConstView 

```C++
inline MUDA_GENERIC muda::TripletMatrixViewBase< IsConst, Ty, 1 >::operator ConstView () const
```




<hr>



### function row\_indices [1/2]

```C++
inline MUDA_GENERIC auto_const_t< int > * muda::TripletMatrixViewBase< IsConst, Ty, 1 >::row_indices () 
```




<hr>



### function row\_indices [2/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::row_indices () const
```




<hr>



### function submatrix 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::submatrix (
    int2 offset,
    int2 extent
) const
```




<hr>



### function submatrix\_offset 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::submatrix_offset () const
```




<hr>



### function subview [1/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::subview (
    int offset,
    int count
) const
```




<hr>



### function subview [2/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::subview (
    int offset
) const
```




<hr>



### function total\_cols 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::total_cols () const
```




<hr>



### function total\_extent 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::total_extent () const
```




<hr>



### function total\_rows 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::total_rows () const
```




<hr>



### function total\_triplet\_count 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::total_triplet_count () const
```




<hr>



### function tripet\_index\_offset 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::tripet_index_offset () const
```




<hr>



### function triplet\_count 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::triplet_count () const
```




<hr>



### function values [1/2]

```C++
inline MUDA_GENERIC auto_const_t< Ty > * muda::TripletMatrixViewBase< IsConst, Ty, 1 >::values () 
```




<hr>



### function values [2/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::values () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase< IsConst, Ty, 1 >::viewer () 
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, 1 >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_indices 

```C++
auto_const_t<int>* muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_col_indices;
```




<hr>



### variable m\_row\_indices 

```C++
auto_const_t<int>* muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_row_indices;
```




<hr>



### variable m\_submatrix\_extent 

```C++
int2 muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_submatrix_extent;
```




<hr>



### variable m\_submatrix\_offset 

```C++
int2 muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_submatrix_offset;
```




<hr>



### variable m\_total\_cols 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_total_cols;
```




<hr>



### variable m\_total\_rows 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_total_rows;
```




<hr>



### variable m\_total\_triplet\_count 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_total_triplet_count;
```




<hr>



### variable m\_triplet\_count 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_triplet_count;
```




<hr>



### variable m\_triplet\_index\_offset 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_triplet_index_offset;
```




<hr>



### variable m\_values 

```C++
auto_const_t<Ty>* muda::TripletMatrixViewBase< IsConst, Ty, 1 >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/triplet_matrix_view.h`

