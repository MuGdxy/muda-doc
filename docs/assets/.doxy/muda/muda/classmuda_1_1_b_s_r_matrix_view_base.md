

# Class muda::BSRMatrixViewBase

**template &lt;bool IsConst, typename Ty, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**BSRMatrixViewBase**](classmuda_1_1_b_s_r_matrix_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; Ty, N, N &gt; | [**BlockMatrix**](#typedef-blockmatrix)  <br> |
| typedef [**BSRMatrixViewBase**](classmuda_1_1_b_s_r_matrix_view_base.md)&lt; true, Ty, N &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**BSRMatrixViewBase**](classmuda_1_1_b_s_r_matrix_view_base.md)&lt; false, Ty, N &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**BSRMatrixViewBase**](classmuda_1_1_b_s_r_matrix_view_base.md)&lt; IsConst, Ty, N &gt; | [**ThisView**](#typedef-thisview)  <br> |


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
|   | [**BSRMatrixViewBase**](#function-bsrmatrixviewbase-12) () = default<br> |
|   | [**BSRMatrixViewBase**](#function-bsrmatrixviewbase-22) (int row, int col, auto\_const\_t&lt; int &gt; \* block\_row\_offsets, auto\_const\_t&lt; int &gt; \* block\_col\_indices, auto\_const\_t&lt; BlockMatrix &gt; \* block\_values, int non\_zeros, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) <br> |
|  auto | [**T**](#function-t) () const<br> |
|  [**ConstView**](classmuda_1_1_b_s_r_matrix_view_base.md) | [**as\_const**](#function-as_const) () const<br> |
|  auto\_const\_t&lt; int &gt; \* | [**block\_col\_indices**](#function-block_col_indices-12) () <br> |
|  auto | [**block\_col\_indices**](#function-block_col_indices-22) () const<br> |
|  auto | [**block\_cols**](#function-block_cols) () const<br> |
|  auto\_const\_t&lt; int &gt; \* | [**block\_row\_offsets**](#function-block_row_offsets-12) () <br> |
|  auto | [**block\_row\_offsets**](#function-block_row_offsets-22) () const<br> |
|  auto | [**block\_rows**](#function-block_rows) () const<br> |
|  auto\_const\_t&lt; BlockMatrix &gt; \* | [**block\_values**](#function-block_values-12) () <br> |
|  auto | [**block\_values**](#function-block_values-22) () const<br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**is\_trans**](#function-is_trans) () const<br> |
|  auto | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  auto | [**non\_zero\_blocks**](#function-non_zero_blocks) () const<br> |
|   | [**operator ConstView**](#function-operator-constview) () const<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; int &gt; \* | [**m\_block\_col\_indices**](#variable-m_block_col_indices)   = = nullptr<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_block\_row\_offsets**](#variable-m_block_row_offsets)   = = nullptr<br> |
|  auto\_const\_t&lt; BlockMatrix &gt; \* | [**m\_block\_values**](#variable-m_block_values)   = = nullptr<br> |
|  int | [**m\_col**](#variable-m_col)   = = 0<br> |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |
|  int | [**m\_non\_zeros**](#variable-m_non_zeros)   = = 0<br> |
|  int | [**m\_row**](#variable-m_row)   = = 0<br> |
|  bool | [**m\_trans**](#variable-m_trans)   = = false<br> |








































## Public Types Documentation




### typedef BlockMatrix 

```C++
using muda::BSRMatrixViewBase< IsConst, Ty, N >::BlockMatrix =  Eigen::Matrix<Ty, N, N>;
```




<hr>



### typedef ConstView 

```C++
using muda::BSRMatrixViewBase< IsConst, Ty, N >::ConstView =  BSRMatrixViewBase<true, Ty, N>;
```




<hr>



### typedef NonConstView 

```C++
using muda::BSRMatrixViewBase< IsConst, Ty, N >::NonConstView =  BSRMatrixViewBase<false, Ty, N>;
```




<hr>



### typedef ThisView 

```C++
using muda::BSRMatrixViewBase< IsConst, Ty, N >::ThisView =  BSRMatrixViewBase<IsConst, Ty, N>;
```




<hr>
## Public Functions Documentation




### function BSRMatrixViewBase [1/2]

```C++
muda::BSRMatrixViewBase::BSRMatrixViewBase () = default
```




<hr>



### function BSRMatrixViewBase [2/2]

```C++
inline muda::BSRMatrixViewBase::BSRMatrixViewBase (
    int row,
    int col,
    auto_const_t< int > * block_row_offsets,
    auto_const_t< int > * block_col_indices,
    auto_const_t< BlockMatrix > * block_values,
    int non_zeros,
    cusparseSpMatDescr_t descr,
    cusparseMatDescr_t legacy_descr,
    bool trans
) 
```




<hr>



### function T 

```C++
inline auto muda::BSRMatrixViewBase::T () const
```




<hr>



### function as\_const 

```C++
inline ConstView muda::BSRMatrixViewBase::as_const () const
```




<hr>



### function block\_col\_indices [1/2]

```C++
inline auto_const_t< int > * muda::BSRMatrixViewBase::block_col_indices () 
```




<hr>



### function block\_col\_indices [2/2]

```C++
inline auto muda::BSRMatrixViewBase::block_col_indices () const
```




<hr>



### function block\_cols 

```C++
inline auto muda::BSRMatrixViewBase::block_cols () const
```




<hr>



### function block\_row\_offsets [1/2]

```C++
inline auto_const_t< int > * muda::BSRMatrixViewBase::block_row_offsets () 
```




<hr>



### function block\_row\_offsets [2/2]

```C++
inline auto muda::BSRMatrixViewBase::block_row_offsets () const
```




<hr>



### function block\_rows 

```C++
inline auto muda::BSRMatrixViewBase::block_rows () const
```




<hr>



### function block\_values [1/2]

```C++
inline auto_const_t< BlockMatrix > * muda::BSRMatrixViewBase::block_values () 
```




<hr>



### function block\_values [2/2]

```C++
inline auto muda::BSRMatrixViewBase::block_values () const
```




<hr>



### function descr 

```C++
inline auto muda::BSRMatrixViewBase::descr () const
```




<hr>



### function is\_trans 

```C++
inline auto muda::BSRMatrixViewBase::is_trans () const
```




<hr>



### function legacy\_descr 

```C++
inline auto muda::BSRMatrixViewBase::legacy_descr () const
```




<hr>



### function non\_zero\_blocks 

```C++
inline auto muda::BSRMatrixViewBase::non_zero_blocks () const
```




<hr>



### function operator ConstView 

```C++
inline muda::BSRMatrixViewBase::operator ConstView () const
```




<hr>
## Protected Attributes Documentation




### variable m\_block\_col\_indices 

```C++
auto_const_t<int>* muda::BSRMatrixViewBase< IsConst, Ty, N >::m_block_col_indices;
```




<hr>



### variable m\_block\_row\_offsets 

```C++
auto_const_t<int>* muda::BSRMatrixViewBase< IsConst, Ty, N >::m_block_row_offsets;
```




<hr>



### variable m\_block\_values 

```C++
auto_const_t<BlockMatrix>* muda::BSRMatrixViewBase< IsConst, Ty, N >::m_block_values;
```




<hr>



### variable m\_col 

```C++
int muda::BSRMatrixViewBase< IsConst, Ty, N >::m_col;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::BSRMatrixViewBase< IsConst, Ty, N >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::BSRMatrixViewBase< IsConst, Ty, N >::m_legacy_descr;
```




<hr>



### variable m\_non\_zeros 

```C++
int muda::BSRMatrixViewBase< IsConst, Ty, N >::m_non_zeros;
```




<hr>



### variable m\_row 

```C++
int muda::BSRMatrixViewBase< IsConst, Ty, N >::m_row;
```




<hr>



### variable m\_trans 

```C++
bool muda::BSRMatrixViewBase< IsConst, Ty, N >::m_trans;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/bsr_matrix_view.h`

