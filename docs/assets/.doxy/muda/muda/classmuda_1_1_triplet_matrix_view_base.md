

# Class muda::TripletMatrixViewBase

**template &lt;bool IsConst, typename Ty, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; Ty, N, N &gt; | [**BlockMatrix**](#typedef-blockmatrix)  <br> |
| typedef [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)&lt; true, Ty, N &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)&lt; false, Ty, N &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**TripletMatrixViewBase**](classmuda_1_1_triplet_matrix_view_base.md)&lt; IsConst, Ty, N &gt; | [**ThisView**](#typedef-thisview)  <br> |


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
|  MUDA\_GENERIC | [**TripletMatrixViewBase**](#function-tripletmatrixviewbase-23) (int total\_block\_rows, int total\_block\_cols, int triplet\_index\_offset, int triplet\_count, int total\_triplet\_count, int2 submatrix\_offset, int2 submatrix\_extent, auto\_const\_t&lt; int &gt; \* block\_row\_indices, auto\_const\_t&lt; int &gt; \* block\_col\_indices, auto\_const\_t&lt; BlockMatrix &gt; \* block\_values) <br> |
|  MUDA\_GENERIC | [**TripletMatrixViewBase**](#function-tripletmatrixviewbase-33) (int total\_block\_rows, int total\_block\_cols, int total\_triplet\_count, auto\_const\_t&lt; int &gt; \* block\_row\_indices, auto\_const\_t&lt; int &gt; \* block\_col\_indices, auto\_const\_t&lt; BlockMatrix &gt; \* block\_values) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_triplet_matrix_view_base.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; int &gt; \* | [**block\_col\_indices**](#function-block_col_indices) () <br> |
|  MUDA\_GENERIC auto\_const\_t&lt; int &gt; \* | [**block\_row\_indices**](#function-block_row_indices) () <br> |
|  MUDA\_GENERIC auto\_const\_t&lt; BlockMatrix &gt; \* | [**block\_values**](#function-block_values) () <br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto | [**extent**](#function-extent) () const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](#function-operator-constview) () const<br> |
|  MUDA\_GENERIC auto | [**submatrix**](#function-submatrix) (int2 offset, int2 extent) const<br> |
|  MUDA\_GENERIC auto | [**submatrix\_offset**](#function-submatrix_offset) () const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-12) (int offset, int count) const<br> |
|  MUDA\_GENERIC auto | [**subview**](#function-subview-22) (int offset) const<br> |
|  MUDA\_GENERIC auto | [**total\_block\_cols**](#function-total_block_cols) () const<br> |
|  MUDA\_GENERIC auto | [**total\_block\_rows**](#function-total_block_rows) () const<br> |
|  MUDA\_GENERIC auto | [**total\_extent**](#function-total_extent) () const<br> |
|  MUDA\_GENERIC auto | [**total\_triplet\_count**](#function-total_triplet_count) () const<br> |
|  MUDA\_GENERIC auto | [**tripet\_index\_offset**](#function-tripet_index_offset) () const<br> |
|  MUDA\_GENERIC auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () <br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; int &gt; \* | [**m\_block\_col\_indices**](#variable-m_block_col_indices)   = = nullptr<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_block\_row\_indices**](#variable-m_block_row_indices)   = = nullptr<br> |
|  auto\_const\_t&lt; BlockMatrix &gt; \* | [**m\_block\_values**](#variable-m_block_values)   = = nullptr<br> |
|  int2 | [**m\_submatrix\_extent**](#variable-m_submatrix_extent)   = = {0, 0}<br> |
|  int2 | [**m\_submatrix\_offset**](#variable-m_submatrix_offset)   = = {0, 0}<br> |
|  int | [**m\_total\_block\_cols**](#variable-m_total_block_cols)   = = 0<br> |
|  int | [**m\_total\_block\_rows**](#variable-m_total_block_rows)   = = 0<br> |
|  int | [**m\_total\_triplet\_count**](#variable-m_total_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_count**](#variable-m_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_index\_offset**](#variable-m_triplet_index_offset)   = = 0<br> |








































## Public Types Documentation




### typedef BlockMatrix 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, N >::BlockMatrix =  Eigen::Matrix<Ty, N, N>;
```




<hr>



### typedef ConstView 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, N >::ConstView =  TripletMatrixViewBase<true, Ty, N>;
```




<hr>



### typedef NonConstView 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, N >::NonConstView =  TripletMatrixViewBase<false, Ty, N>;
```




<hr>



### typedef ThisView 

```C++
using muda::TripletMatrixViewBase< IsConst, Ty, N >::ThisView =  TripletMatrixViewBase<IsConst, Ty, N>;
```




<hr>
## Public Functions Documentation




### function TripletMatrixViewBase [1/3]

```C++
MUDA_GENERIC muda::TripletMatrixViewBase::TripletMatrixViewBase () = default
```




<hr>



### function TripletMatrixViewBase [2/3]

```C++
inline MUDA_GENERIC muda::TripletMatrixViewBase::TripletMatrixViewBase (
    int total_block_rows,
    int total_block_cols,
    int triplet_index_offset,
    int triplet_count,
    int total_triplet_count,
    int2 submatrix_offset,
    int2 submatrix_extent,
    auto_const_t< int > * block_row_indices,
    auto_const_t< int > * block_col_indices,
    auto_const_t< BlockMatrix > * block_values
) 
```




<hr>



### function TripletMatrixViewBase [3/3]

```C++
inline MUDA_GENERIC muda::TripletMatrixViewBase::TripletMatrixViewBase (
    int total_block_rows,
    int total_block_cols,
    int total_triplet_count,
    auto_const_t< int > * block_row_indices,
    auto_const_t< int > * block_col_indices,
    auto_const_t< BlockMatrix > * block_values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstView muda::TripletMatrixViewBase::as_const () const
```




<hr>



### function block\_col\_indices 

```C++
inline MUDA_GENERIC auto_const_t< int > * muda::TripletMatrixViewBase::block_col_indices () 
```




<hr>



### function block\_row\_indices 

```C++
inline MUDA_GENERIC auto_const_t< int > * muda::TripletMatrixViewBase::block_row_indices () 
```




<hr>



### function block\_values 

```C++
inline MUDA_GENERIC auto_const_t< BlockMatrix > * muda::TripletMatrixViewBase::block_values () 
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::cviewer () const
```




<hr>



### function extent 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::extent () const
```




<hr>



### function operator ConstView 

```C++
inline MUDA_GENERIC muda::TripletMatrixViewBase::operator ConstView () const
```




<hr>



### function submatrix 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::submatrix (
    int2 offset,
    int2 extent
) const
```




<hr>



### function submatrix\_offset 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::submatrix_offset () const
```




<hr>



### function subview [1/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::subview (
    int offset,
    int count
) const
```




<hr>



### function subview [2/2]

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::subview (
    int offset
) const
```




<hr>



### function total\_block\_cols 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::total_block_cols () const
```




<hr>



### function total\_block\_rows 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::total_block_rows () const
```




<hr>



### function total\_extent 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::total_extent () const
```




<hr>



### function total\_triplet\_count 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::total_triplet_count () const
```




<hr>



### function tripet\_index\_offset 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::tripet_index_offset () const
```




<hr>



### function triplet\_count 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::triplet_count () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::TripletMatrixViewBase::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_block\_col\_indices 

```C++
auto_const_t<int>* muda::TripletMatrixViewBase< IsConst, Ty, N >::m_block_col_indices;
```




<hr>



### variable m\_block\_row\_indices 

```C++
auto_const_t<int>* muda::TripletMatrixViewBase< IsConst, Ty, N >::m_block_row_indices;
```




<hr>



### variable m\_block\_values 

```C++
auto_const_t<BlockMatrix>* muda::TripletMatrixViewBase< IsConst, Ty, N >::m_block_values;
```




<hr>



### variable m\_submatrix\_extent 

```C++
int2 muda::TripletMatrixViewBase< IsConst, Ty, N >::m_submatrix_extent;
```




<hr>



### variable m\_submatrix\_offset 

```C++
int2 muda::TripletMatrixViewBase< IsConst, Ty, N >::m_submatrix_offset;
```




<hr>



### variable m\_total\_block\_cols 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, N >::m_total_block_cols;
```




<hr>



### variable m\_total\_block\_rows 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, N >::m_total_block_rows;
```




<hr>



### variable m\_total\_triplet\_count 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, N >::m_total_triplet_count;
```




<hr>



### variable m\_triplet\_count 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, N >::m_triplet_count;
```




<hr>



### variable m\_triplet\_index\_offset 

```C++
int muda::TripletMatrixViewBase< IsConst, Ty, N >::m_triplet_index_offset;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/triplet_matrix_view.h`

