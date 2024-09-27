

# Class muda::COOMatrixViewBase

**template &lt;bool IsConst, typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**COOMatrixViewBase**](classmuda_1_1_c_o_o_matrix_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**COOMatrixViewBase**](classmuda_1_1_c_o_o_matrix_view_base.md)&lt; true, Ty &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**COOMatrixViewBase**](classmuda_1_1_c_o_o_matrix_view_base.md)&lt; false, Ty &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**COOMatrixViewBase**](classmuda_1_1_c_o_o_matrix_view_base.md)&lt; IsConst, Ty &gt; | [**ThisView**](#typedef-thisview)  <br> |


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
|  MUDA\_GENERIC | [**COOMatrixViewBase**](#function-coomatrixviewbase-13) () = default<br> |
|  MUDA\_GENERIC | [**COOMatrixViewBase**](#function-coomatrixviewbase-23) (int rows, int cols, int triplet\_index\_offset, int triplet\_count, int total\_triplet\_count, int2 submatrix\_offset, int2 submatrix\_extent, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) <br> |
|  MUDA\_GENERIC | [**COOMatrixViewBase**](#function-coomatrixviewbase-33) (int rows, int cols, int total\_triplet\_count, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  auto\_const\_t&lt; int &gt; \* | [**block\_col\_indices**](#function-block_col_indices-12) () <br> |
|  auto | [**block\_col\_indices**](#function-block_col_indices-22) () const<br> |
|  auto | [**block\_cols**](#function-block_cols) () const<br> |
|  auto\_const\_t&lt; int &gt; \* | [**block\_row\_indices**](#function-block_row_indices-12) () <br> |
|  auto | [**block\_row\_indices**](#function-block_row_indices-22) () const<br> |
|  auto | [**block\_rows**](#function-block_rows) () const<br> |
|  auto\_const\_t&lt; Ty &gt; \* | [**block\_values**](#function-block_values-12) () <br> |
|  auto | [**block\_values**](#function-block_values-22) () const<br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**is\_trans**](#function-is_trans) () const<br> |
|  auto | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](#function-operator-constview) () const<br> |
|  auto | [**total\_triplet\_count**](#function-total_triplet_count) () const<br> |
|  auto | [**tripet\_index\_offset**](#function-tripet_index_offset) () const<br> |
|  auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () <br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; int &gt; \* | [**m\_col\_indices**](#variable-m_col_indices)  <br> |
|  int | [**m\_cols**](#variable-m_cols)   = = 0<br> |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_row\_indices**](#variable-m_row_indices)  <br> |
|  int | [**m\_rows**](#variable-m_rows)   = = 0<br> |
|  int2 | [**m\_submatrix\_extent**](#variable-m_submatrix_extent)   = = {0, 0}<br> |
|  int2 | [**m\_submatrix\_offset**](#variable-m_submatrix_offset)   = = {0, 0}<br> |
|  int | [**m\_total\_triplet\_count**](#variable-m_total_triplet_count)   = = 0<br> |
|  bool | [**m\_trans**](#variable-m_trans)   = = false<br> |
|  int | [**m\_triplet\_count**](#variable-m_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_index\_offset**](#variable-m_triplet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; Ty &gt; \* | [**m\_values**](#variable-m_values)  <br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::COOMatrixViewBase< IsConst, Ty >::ConstView =  COOMatrixViewBase<true, Ty>;
```




<hr>



### typedef NonConstView 

```C++
using muda::COOMatrixViewBase< IsConst, Ty >::NonConstView =  COOMatrixViewBase<false, Ty>;
```




<hr>



### typedef ThisView 

```C++
using muda::COOMatrixViewBase< IsConst, Ty >::ThisView =  COOMatrixViewBase<IsConst, Ty>;
```




<hr>
## Public Functions Documentation




### function COOMatrixViewBase [1/3]

```C++
MUDA_GENERIC muda::COOMatrixViewBase::COOMatrixViewBase () = default
```




<hr>



### function COOMatrixViewBase [2/3]

```C++
inline MUDA_GENERIC muda::COOMatrixViewBase::COOMatrixViewBase (
    int rows,
    int cols,
    int triplet_index_offset,
    int triplet_count,
    int total_triplet_count,
    int2 submatrix_offset,
    int2 submatrix_extent,
    auto_const_t< int > * row_indices,
    auto_const_t< int > * col_indices,
    auto_const_t< Ty > * values,
    cusparseSpMatDescr_t descr,
    cusparseMatDescr_t legacy_descr,
    bool trans
) 
```




<hr>



### function COOMatrixViewBase [3/3]

```C++
inline MUDA_GENERIC muda::COOMatrixViewBase::COOMatrixViewBase (
    int rows,
    int cols,
    int total_triplet_count,
    auto_const_t< int > * row_indices,
    auto_const_t< int > * col_indices,
    auto_const_t< Ty > * values,
    cusparseSpMatDescr_t descr,
    cusparseMatDescr_t legacy_descr,
    bool trans
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::COOMatrixViewBase::as_const () const
```




<hr>



### function block\_col\_indices [1/2]

```C++
inline auto_const_t< int > * muda::COOMatrixViewBase::block_col_indices () 
```




<hr>



### function block\_col\_indices [2/2]

```C++
inline auto muda::COOMatrixViewBase::block_col_indices () const
```




<hr>



### function block\_cols 

```C++
inline auto muda::COOMatrixViewBase::block_cols () const
```




<hr>



### function block\_row\_indices [1/2]

```C++
inline auto_const_t< int > * muda::COOMatrixViewBase::block_row_indices () 
```




<hr>



### function block\_row\_indices [2/2]

```C++
inline auto muda::COOMatrixViewBase::block_row_indices () const
```




<hr>



### function block\_rows 

```C++
inline auto muda::COOMatrixViewBase::block_rows () const
```




<hr>



### function block\_values [1/2]

```C++
inline auto_const_t< Ty > * muda::COOMatrixViewBase::block_values () 
```




<hr>



### function block\_values [2/2]

```C++
inline auto muda::COOMatrixViewBase::block_values () const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::COOMatrixViewBase::cviewer () const
```




<hr>



### function descr 

```C++
inline auto muda::COOMatrixViewBase::descr () const
```




<hr>



### function is\_trans 

```C++
inline auto muda::COOMatrixViewBase::is_trans () const
```




<hr>



### function legacy\_descr 

```C++
inline auto muda::COOMatrixViewBase::legacy_descr () const
```




<hr>



### function operator ConstView 

```C++
inline MUDA_GENERIC muda::COOMatrixViewBase::operator ConstView () const
```




<hr>



### function total\_triplet\_count 

```C++
inline auto muda::COOMatrixViewBase::total_triplet_count () const
```




<hr>



### function tripet\_index\_offset 

```C++
inline auto muda::COOMatrixViewBase::tripet_index_offset () const
```




<hr>



### function triplet\_count 

```C++
inline auto muda::COOMatrixViewBase::triplet_count () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::COOMatrixViewBase::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_indices 

```C++
auto_const_t<int>* muda::COOMatrixViewBase< IsConst, Ty >::m_col_indices;
```




<hr>



### variable m\_cols 

```C++
int muda::COOMatrixViewBase< IsConst, Ty >::m_cols;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::COOMatrixViewBase< IsConst, Ty >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::COOMatrixViewBase< IsConst, Ty >::m_legacy_descr;
```




<hr>



### variable m\_row\_indices 

```C++
auto_const_t<int>* muda::COOMatrixViewBase< IsConst, Ty >::m_row_indices;
```




<hr>



### variable m\_rows 

```C++
int muda::COOMatrixViewBase< IsConst, Ty >::m_rows;
```




<hr>



### variable m\_submatrix\_extent 

```C++
int2 muda::COOMatrixViewBase< IsConst, Ty >::m_submatrix_extent;
```




<hr>



### variable m\_submatrix\_offset 

```C++
int2 muda::COOMatrixViewBase< IsConst, Ty >::m_submatrix_offset;
```




<hr>



### variable m\_total\_triplet\_count 

```C++
int muda::COOMatrixViewBase< IsConst, Ty >::m_total_triplet_count;
```




<hr>



### variable m\_trans 

```C++
bool muda::COOMatrixViewBase< IsConst, Ty >::m_trans;
```




<hr>



### variable m\_triplet\_count 

```C++
int muda::COOMatrixViewBase< IsConst, Ty >::m_triplet_count;
```




<hr>



### variable m\_triplet\_index\_offset 

```C++
int muda::COOMatrixViewBase< IsConst, Ty >::m_triplet_index_offset;
```




<hr>



### variable m\_values 

```C++
auto_const_t<Ty>* muda::COOMatrixViewBase< IsConst, Ty >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/bcoo_matrix_view.h`

