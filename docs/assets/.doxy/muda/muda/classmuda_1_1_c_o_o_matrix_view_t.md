

# Class muda::COOMatrixViewT

**template &lt;bool IsConst, typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**COOMatrixViewT**](classmuda_1_1_c_o_o_matrix_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**COOMatrixViewT**](classmuda_1_1_c_o_o_matrix_view_t.md)&lt; true, Ty &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**COOMatrixViewT**](classmuda_1_1_c_o_o_matrix_view_t.md)&lt; false, Ty &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef [**COOMatrixViewT**](classmuda_1_1_c_o_o_matrix_view_t.md)&lt; IsConst, Ty &gt; | [**ThisView**](#typedef-thisview)  <br> |


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
|  MUDA\_GENERIC | [**COOMatrixViewT**](#function-coomatrixviewt-25) () = default<br> |
|  MUDA\_GENERIC | [**COOMatrixViewT**](#function-coomatrixviewt-35) (int rows, int cols, int triplet\_index\_offset, int triplet\_count, int total\_triplet\_count, int2 submatrix\_offset, int2 submatrix\_extent, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) <br> |
|  MUDA\_GENERIC | [**COOMatrixViewT**](#function-coomatrixviewt-45) (int rows, int cols, int total\_triplet\_count, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; Ty &gt; \* values, cusparseSpMatDescr\_t descr, cusparseMatDescr\_t legacy\_descr, bool trans) <br> |
|  MUDA\_GENERIC | [**COOMatrixViewT**](#function-coomatrixviewt-55) (const [**COOMatrixViewT**](classmuda_1_1_c_o_o_matrix_view_t.md)&lt; OtherIsConst, Ty &gt; & other) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  auto | [**col\_indices**](#function-col_indices) () const<br> |
|  auto | [**cols**](#function-cols) () const<br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () const<br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**is\_trans**](#function-is_trans) () const<br> |
|  auto | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  auto | [**row\_indices**](#function-row_indices) () const<br> |
|  auto | [**rows**](#function-rows) () const<br> |
|  auto | [**total\_triplet\_count**](#function-total_triplet_count) () const<br> |
|  auto | [**tripet\_index\_offset**](#function-tripet_index_offset) () const<br> |
|  auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  auto | [**values**](#function-values) () const<br> |
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
using muda::COOMatrixViewT< IsConst, Ty >::ConstView =  COOMatrixViewT<true, Ty>;
```




<hr>



### typedef NonConstView 

```C++
using muda::COOMatrixViewT< IsConst, Ty >::NonConstView =  COOMatrixViewT<false, Ty>;
```




<hr>



### typedef ThisView 

```C++
using muda::COOMatrixViewT< IsConst, Ty >::ThisView =  COOMatrixViewT<IsConst, Ty>;
```




<hr>
## Public Functions Documentation




### function COOMatrixViewT [2/5]

```C++
MUDA_GENERIC muda::COOMatrixViewT::COOMatrixViewT () = default
```




<hr>



### function COOMatrixViewT [3/5]

```C++
inline MUDA_GENERIC muda::COOMatrixViewT::COOMatrixViewT (
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



### function COOMatrixViewT [4/5]

```C++
inline MUDA_GENERIC muda::COOMatrixViewT::COOMatrixViewT (
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



### function COOMatrixViewT [5/5]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::COOMatrixViewT::COOMatrixViewT (
    const COOMatrixViewT < OtherIsConst, Ty > & other
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::COOMatrixViewT::as_const () const
```




<hr>



### function col\_indices 

```C++
inline auto muda::COOMatrixViewT::col_indices () const
```




<hr>



### function cols 

```C++
inline auto muda::COOMatrixViewT::cols () const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::COOMatrixViewT::cviewer () const
```




<hr>



### function descr 

```C++
inline auto muda::COOMatrixViewT::descr () const
```




<hr>



### function is\_trans 

```C++
inline auto muda::COOMatrixViewT::is_trans () const
```




<hr>



### function legacy\_descr 

```C++
inline auto muda::COOMatrixViewT::legacy_descr () const
```




<hr>



### function row\_indices 

```C++
inline auto muda::COOMatrixViewT::row_indices () const
```




<hr>



### function rows 

```C++
inline auto muda::COOMatrixViewT::rows () const
```




<hr>



### function total\_triplet\_count 

```C++
inline auto muda::COOMatrixViewT::total_triplet_count () const
```




<hr>



### function tripet\_index\_offset 

```C++
inline auto muda::COOMatrixViewT::tripet_index_offset () const
```




<hr>



### function triplet\_count 

```C++
inline auto muda::COOMatrixViewT::triplet_count () const
```




<hr>



### function values 

```C++
inline auto muda::COOMatrixViewT::values () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::COOMatrixViewT::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_indices 

```C++
auto_const_t<int>* muda::COOMatrixViewT< IsConst, Ty >::m_col_indices;
```




<hr>



### variable m\_cols 

```C++
int muda::COOMatrixViewT< IsConst, Ty >::m_cols;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::COOMatrixViewT< IsConst, Ty >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::COOMatrixViewT< IsConst, Ty >::m_legacy_descr;
```




<hr>



### variable m\_row\_indices 

```C++
auto_const_t<int>* muda::COOMatrixViewT< IsConst, Ty >::m_row_indices;
```




<hr>



### variable m\_rows 

```C++
int muda::COOMatrixViewT< IsConst, Ty >::m_rows;
```




<hr>



### variable m\_submatrix\_extent 

```C++
int2 muda::COOMatrixViewT< IsConst, Ty >::m_submatrix_extent;
```




<hr>



### variable m\_submatrix\_offset 

```C++
int2 muda::COOMatrixViewT< IsConst, Ty >::m_submatrix_offset;
```




<hr>



### variable m\_total\_triplet\_count 

```C++
int muda::COOMatrixViewT< IsConst, Ty >::m_total_triplet_count;
```




<hr>



### variable m\_trans 

```C++
bool muda::COOMatrixViewT< IsConst, Ty >::m_trans;
```




<hr>



### variable m\_triplet\_count 

```C++
int muda::COOMatrixViewT< IsConst, Ty >::m_triplet_count;
```




<hr>



### variable m\_triplet\_index\_offset 

```C++
int muda::COOMatrixViewT< IsConst, Ty >::m_triplet_index_offset;
```




<hr>



### variable m\_values 

```C++
auto_const_t<Ty>* muda::COOMatrixViewT< IsConst, Ty >::m_values;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/bcoo_matrix_view.h`

