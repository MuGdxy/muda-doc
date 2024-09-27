

# Class muda::CSRMatrixViewBase

**template &lt;bool IsConst, typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**CSRMatrixViewBase**](classmuda_1_1_c_s_r_matrix_view_base.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**CSRMatrixViewBase**](classmuda_1_1_c_s_r_matrix_view_base.md)&lt; true, Ty &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**CSRMatrixViewBase**](classmuda_1_1_c_s_r_matrix_view_base.md)&lt; false, Ty &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**CSRMatrixViewBase**](classmuda_1_1_c_s_r_matrix_view_base.md)&lt; IsConst, Ty &gt; | [**ThisView**](#typedef-thisview)  <br> |


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
|   | [**CSRMatrixViewBase**](#function-csrmatrixviewbase-12) () = default<br> |
|   | [**CSRMatrixViewBase**](#function-csrmatrixviewbase-22) (int row, int col, auto\_const\_t&lt; int &gt; \* row\_offsets, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values, int non\_zero, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) <br> |
|  auto | [**T**](#function-t) () const<br> |
|  [**ConstView**](classmuda_1_1_c_s_r_matrix_view_base.md) | [**as\_const**](#function-as_const) () const<br> |
|  auto\_const\_t&lt; int &gt; \* | [**col\_indices**](#function-col_indices-12) () <br> |
|  auto | [**col\_indices**](#function-col_indices-22) () const<br> |
|  auto | [**cols**](#function-cols) () const<br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**is\_trans**](#function-is_trans) () const<br> |
|  auto | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  auto | [**non\_zeros**](#function-non_zeros) () const<br> |
|   | [**operator ConstView**](#function-operator-constview) () const<br> |
|  auto\_const\_t&lt; int &gt; \* | [**row\_offsets**](#function-row_offsets-12) () <br> |
|  auto | [**row\_offsets**](#function-row_offsets-22) () const<br> |
|  auto | [**rows**](#function-rows) () const<br> |
|  auto\_const\_t&lt; Ty &gt; \* | [**values**](#function-values-12) () <br> |
|  auto | [**values**](#function-values-22) () const<br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_col**](#variable-m_col)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_col\_indices**](#variable-m_col_indices)   = = nullptr<br> |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |
|  int | [**m\_non\_zero**](#variable-m_non_zero)   = = 0<br> |
|  int | [**m\_row**](#variable-m_row)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_row\_offsets**](#variable-m_row_offsets)   = = nullptr<br> |
|  bool | [**m\_trans**](#variable-m_trans)   = = false<br> |
|  auto\_const\_t&lt; Ty &gt; \* | [**m\_values**](#variable-m_values)   = = nullptr<br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::CSRMatrixViewBase< IsConst, Ty >::ConstView =  CSRMatrixViewBase<true, Ty>;
```




<hr>



### typedef NonConstView 

```C++
using muda::CSRMatrixViewBase< IsConst, Ty >::NonConstView =  CSRMatrixViewBase<false, Ty>;
```




<hr>



### typedef ThisView 

```C++
using muda::CSRMatrixViewBase< IsConst, Ty >::ThisView =  CSRMatrixViewBase<IsConst, Ty>;
```




<hr>
## Public Functions Documentation




### function CSRMatrixViewBase [1/2]

```C++
muda::CSRMatrixViewBase::CSRMatrixViewBase () = default
```




<hr>



### function CSRMatrixViewBase [2/2]

```C++
inline muda::CSRMatrixViewBase::CSRMatrixViewBase (
    int row,
    int col,
    auto_const_t< int > * row_offsets,
    auto_const_t< int > * col_indices,
    auto_const_t< Ty > * values,
    int non_zero,
    cusparseSpMatDescr_t descr,
    cusparseMatDescr_t legacy_descr,
    bool trans
) 
```




<hr>



### function T 

```C++
inline auto muda::CSRMatrixViewBase::T () const
```




<hr>



### function as\_const 

```C++
inline ConstView muda::CSRMatrixViewBase::as_const () const
```




<hr>



### function col\_indices [1/2]

```C++
inline auto_const_t< int > * muda::CSRMatrixViewBase::col_indices () 
```




<hr>



### function col\_indices [2/2]

```C++
inline auto muda::CSRMatrixViewBase::col_indices () const
```




<hr>



### function cols 

```C++
inline auto muda::CSRMatrixViewBase::cols () const
```




<hr>



### function descr 

```C++
inline auto muda::CSRMatrixViewBase::descr () const
```




<hr>



### function is\_trans 

```C++
inline auto muda::CSRMatrixViewBase::is_trans () const
```




<hr>



### function legacy\_descr 

```C++
inline auto muda::CSRMatrixViewBase::legacy_descr () const
```




<hr>



### function non\_zeros 

```C++
inline auto muda::CSRMatrixViewBase::non_zeros () const
```




<hr>



### function operator ConstView 

```C++
inline muda::CSRMatrixViewBase::operator ConstView () const
```




<hr>



### function row\_offsets [1/2]

```C++
inline auto_const_t< int > * muda::CSRMatrixViewBase::row_offsets () 
```




<hr>



### function row\_offsets [2/2]

```C++
inline auto muda::CSRMatrixViewBase::row_offsets () const
```




<hr>



### function rows 

```C++
inline auto muda::CSRMatrixViewBase::rows () const
```




<hr>



### function values [1/2]

```C++
inline auto_const_t< Ty > * muda::CSRMatrixViewBase::values () 
```




<hr>



### function values [2/2]

```C++
inline auto muda::CSRMatrixViewBase::values () const
```




<hr>
## Protected Attributes Documentation




### variable m\_col 

```C++
int muda::CSRMatrixViewBase< IsConst, Ty >::m_col;
```




<hr>



### variable m\_col\_indices 

```C++
auto_const_t<int>* muda::CSRMatrixViewBase< IsConst, Ty >::m_col_indices;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::CSRMatrixViewBase< IsConst, Ty >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::CSRMatrixViewBase< IsConst, Ty >::m_legacy_descr;
```




<hr>



### variable m\_non\_zero 

```C++
int muda::CSRMatrixViewBase< IsConst, Ty >::m_non_zero;
```




<hr>



### variable m\_row 

```C++
int muda::CSRMatrixViewBase< IsConst, Ty >::m_row;
```




<hr>



### variable m\_row\_offsets 

```C++
auto_const_t<int>* muda::CSRMatrixViewBase< IsConst, Ty >::m_row_offsets;
```




<hr>



### variable m\_trans 

```C++
bool muda::CSRMatrixViewBase< IsConst, Ty >::m_trans;
```




<hr>



### variable m\_values 

```C++
auto_const_t<Ty>* muda::CSRMatrixViewBase< IsConst, Ty >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/csr_matrix_view.h`

