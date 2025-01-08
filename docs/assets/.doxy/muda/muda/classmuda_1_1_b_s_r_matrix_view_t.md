

# Class muda::BSRMatrixViewT

**template &lt;bool IsConst, typename Ty, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**BSRMatrixViewT**](classmuda_1_1_b_s_r_matrix_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**BSRMatrixViewT**](classmuda_1_1_b_s_r_matrix_view_t.md)&lt; true, Ty, N &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**BSRMatrixViewT**](classmuda_1_1_b_s_r_matrix_view_t.md)&lt; false, Ty, N &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**BSRMatrixViewT**](classmuda_1_1_b_s_r_matrix_view_t.md)&lt; IsConst, Ty, N &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; N==1, Ty, Eigen::Matrix&lt; Ty, N, N &gt; &gt; | [**ValueT**](#typedef-valuet)  <br> |


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
|  MUDA\_GENERIC | [**BSRMatrixViewT**](#function-bsrmatrixviewt-24) () noexcept<br> |
|  MUDA\_GENERIC | [**BSRMatrixViewT**](#function-bsrmatrixviewt-34) (int row, int col, auto\_const\_t&lt; int &gt; \* block\_row\_offsets, auto\_const\_t&lt; int &gt; \* block\_col\_indices, auto\_const\_t&lt; ValueT &gt; \* block\_values, int non\_zeros, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) noexcept<br> |
|  MUDA\_GENERIC | [**BSRMatrixViewT**](#function-bsrmatrixviewt-44) (const [**BSRMatrixViewT**](classmuda_1_1_b_s_r_matrix_view_t.md)&lt; OtherIsConst, Ty, N &gt; & other) noexcept<br> |
|  MUDA\_GENERIC auto | [**T**](#function-t) () const<br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_b_s_r_matrix_view_t.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto | [**col\_indices**](#function-col_indices) () const<br> |
|  MUDA\_GENERIC auto | [**cols**](#function-cols) () const<br> |
|  MUDA\_GENERIC auto | [**descr**](#function-descr) () const<br> |
|  MUDA\_GENERIC auto | [**is\_trans**](#function-is_trans) () const<br> |
|  MUDA\_GENERIC auto | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  MUDA\_GENERIC auto | [**non\_zeros**](#function-non_zeros) () const<br> |
|  MUDA\_GENERIC auto | [**row\_offsets**](#function-row_offsets) () const<br> |
|  MUDA\_GENERIC auto | [**rows**](#function-rows) () const<br> |
|  MUDA\_GENERIC auto | [**values**](#function-values) () const<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_col**](#variable-m_col)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_col\_indices**](#variable-m_col_indices)   = = nullptr<br> |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |
|  int | [**m\_non\_zeros**](#variable-m_non_zeros)   = = 0<br> |
|  int | [**m\_row**](#variable-m_row)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_row\_offsets**](#variable-m_row_offsets)   = = nullptr<br> |
|  bool | [**m\_trans**](#variable-m_trans)   = = false<br> |
|  auto\_const\_t&lt; ValueT &gt; \* | [**m\_values**](#variable-m_values)   = = nullptr<br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::BSRMatrixViewT< IsConst, Ty, N >::ConstView =  BSRMatrixViewT<true, Ty, N>;
```




<hr>



### typedef NonConstView 

```C++
using muda::BSRMatrixViewT< IsConst, Ty, N >::NonConstView =  BSRMatrixViewT<false, Ty, N>;
```




<hr>



### typedef ThisView 

```C++
using muda::BSRMatrixViewT< IsConst, Ty, N >::ThisView =  BSRMatrixViewT<IsConst, Ty, N>;
```




<hr>



### typedef ValueT 

```C++
using muda::BSRMatrixViewT< IsConst, Ty, N >::ValueT =  std::conditional_t<N == 1, Ty, Eigen::Matrix<Ty, N, N>>;
```




<hr>
## Public Functions Documentation




### function BSRMatrixViewT [2/4]

```C++
MUDA_GENERIC muda::BSRMatrixViewT::BSRMatrixViewT () noexcept
```




<hr>



### function BSRMatrixViewT [3/4]

```C++
inline MUDA_GENERIC muda::BSRMatrixViewT::BSRMatrixViewT (
    int row,
    int col,
    auto_const_t< int > * block_row_offsets,
    auto_const_t< int > * block_col_indices,
    auto_const_t< ValueT > * block_values,
    int non_zeros,
    cusparseSpMatDescr_t descr,
    cusparseMatDescr_t legacy_descr,
    bool trans
) noexcept
```




<hr>



### function BSRMatrixViewT [4/4]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::BSRMatrixViewT::BSRMatrixViewT (
    const BSRMatrixViewT < OtherIsConst, Ty, N > & other
) noexcept
```




<hr>



### function T 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::T () const
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstView muda::BSRMatrixViewT::as_const () const
```




<hr>



### function col\_indices 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::col_indices () const
```




<hr>



### function cols 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::cols () const
```




<hr>



### function descr 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::descr () const
```




<hr>



### function is\_trans 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::is_trans () const
```




<hr>



### function legacy\_descr 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::legacy_descr () const
```




<hr>



### function non\_zeros 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::non_zeros () const
```




<hr>



### function row\_offsets 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::row_offsets () const
```




<hr>



### function rows 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::rows () const
```




<hr>



### function values 

```C++
inline MUDA_GENERIC auto muda::BSRMatrixViewT::values () const
```




<hr>
## Protected Attributes Documentation




### variable m\_col 

```C++
int muda::BSRMatrixViewT< IsConst, Ty, N >::m_col;
```




<hr>



### variable m\_col\_indices 

```C++
auto_const_t<int>* muda::BSRMatrixViewT< IsConst, Ty, N >::m_col_indices;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::BSRMatrixViewT< IsConst, Ty, N >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::BSRMatrixViewT< IsConst, Ty, N >::m_legacy_descr;
```




<hr>



### variable m\_non\_zeros 

```C++
int muda::BSRMatrixViewT< IsConst, Ty, N >::m_non_zeros;
```




<hr>



### variable m\_row 

```C++
int muda::BSRMatrixViewT< IsConst, Ty, N >::m_row;
```




<hr>



### variable m\_row\_offsets 

```C++
auto_const_t<int>* muda::BSRMatrixViewT< IsConst, Ty, N >::m_row_offsets;
```




<hr>



### variable m\_trans 

```C++
bool muda::BSRMatrixViewT< IsConst, Ty, N >::m_trans;
```




<hr>



### variable m\_values 

```C++
auto_const_t<ValueT>* muda::BSRMatrixViewT< IsConst, Ty, N >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/bsr_matrix_view.h`

