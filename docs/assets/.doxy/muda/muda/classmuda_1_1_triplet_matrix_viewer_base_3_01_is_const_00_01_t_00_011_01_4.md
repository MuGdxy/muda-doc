

# Class muda::TripletMatrixViewerBase&lt; IsConst, T, 1 &gt;

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**TripletMatrixViewerBase&lt; IsConst, T, 1 &gt;**](classmuda_1_1_triplet_matrix_viewer_base_3_01_is_const_00_01_t_00_011_01_4.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)












## Classes

| Type | Name |
| ---: | :--- |
| struct | [**CTriplet**](structmuda_1_1_triplet_matrix_viewer_base_3_01_is_const_00_01_t_00_011_01_4_1_1_c_triplet.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md)&lt; true, T, 1 &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md)&lt; false, T, 1 &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md)&lt; IsConst, T, 1 &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**TripletMatrixViewerBase**](#function-tripletmatrixviewerbase-12) () = default<br> |
|  MUDA\_GENERIC | [**TripletMatrixViewerBase**](#function-tripletmatrixviewerbase-22) (int total\_rows, int total\_cols, int triplet\_index\_offset, int triplet\_count, int total\_triplet\_count, int2 submatrix\_offset, int2 submatrix\_extent, auto\_const\_t&lt; int &gt; \* row\_indices, auto\_const\_t&lt; int &gt; \* col\_indices, auto\_const\_t&lt; T &gt; \* values) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_triplet_matrix_viewer_base.md) | [**as\_const**](#function-as_const) () const<br> |
|  auto | [**extent**](#function-extent) () const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC CTriplet | [**operator()**](#function-operator()) (int i) const<br> |
|  auto | [**submatrix\_offset**](#function-submatrix_offset) () const<br> |
|  auto | [**total\_cols**](#function-total_cols) () const<br> |
|  auto | [**total\_extent**](#function-total_extent) () const<br> |
|  auto | [**total\_rows**](#function-total_rows) () const<br> |
|  auto | [**total\_triplet\_count**](#function-total_triplet_count) () const<br> |
|  auto | [**tripet\_index\_offset**](#function-tripet_index_offset) () const<br> |
|  auto | [**triplet\_count**](#function-triplet_count) () const<br> |


## Public Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-13) () <br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-23) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-33) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**copy\_label**](classmuda_1_1_viewer_base.md#function-copy_label) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) & other) <br> |
|  MUDA\_GENERIC const char \* | [**kernel\_file**](classmuda_1_1_viewer_base.md#function-kernel_file) () const<br> |
|  MUDA\_GENERIC int | [**kernel\_line**](classmuda_1_1_viewer_base.md#function-kernel_line) () const<br> |
|  MUDA\_GENERIC const char \* | [**kernel\_name**](classmuda_1_1_viewer_base.md#function-kernel_name) () const<br> |
|  MUDA\_GENERIC const char \* | [**name**](classmuda_1_1_viewer_base.md#function-name-13) () const<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator_1) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |






## Protected Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |


## Protected Types inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_viewer_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_viewer_base.md#typedef-non_const_enable_t)  <br> |






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
|  auto\_const\_t&lt; T &gt; \* | [**m\_values**](#variable-m_values)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_in\_submatrix**](#function-check_in_submatrix) (int i, int j) noexcept const<br> |
|  MUDA\_INLINE MUDA\_GENERIC int | [**get\_index**](#function-get_index) (int i) noexcept const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef ConstViewer 

```C++
using muda::TripletMatrixViewerBase< IsConst, T, 1 >::ConstViewer =  TripletMatrixViewerBase<true, T, 1>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::TripletMatrixViewerBase< IsConst, T, 1 >::NonConstViewer =  TripletMatrixViewerBase<false, T, 1>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::TripletMatrixViewerBase< IsConst, T, 1 >::ThisViewer =  TripletMatrixViewerBase<IsConst, T, 1>;
```




<hr>
## Public Functions Documentation




### function TripletMatrixViewerBase [1/2]

```C++
MUDA_GENERIC muda::TripletMatrixViewerBase< IsConst, T, 1 >::TripletMatrixViewerBase () = default
```




<hr>



### function TripletMatrixViewerBase [2/2]

```C++
inline MUDA_GENERIC muda::TripletMatrixViewerBase< IsConst, T, 1 >::TripletMatrixViewerBase (
    int total_rows,
    int total_cols,
    int triplet_index_offset,
    int triplet_count,
    int total_triplet_count,
    int2 submatrix_offset,
    int2 submatrix_extent,
    auto_const_t< int > * row_indices,
    auto_const_t< int > * col_indices,
    auto_const_t< T > * values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstViewer muda::TripletMatrixViewerBase< IsConst, T, 1 >::as_const () const
```




<hr>



### function extent 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::extent () const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::TripletMatrixViewerBase< IsConst, T, 1 >::operator ConstViewer () const
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC CTriplet muda::TripletMatrixViewerBase< IsConst, T, 1 >::operator() (
    int i
) const
```




<hr>



### function submatrix\_offset 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::submatrix_offset () const
```




<hr>



### function total\_cols 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::total_cols () const
```




<hr>



### function total\_extent 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::total_extent () const
```




<hr>



### function total\_rows 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::total_rows () const
```




<hr>



### function total\_triplet\_count 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::total_triplet_count () const
```




<hr>



### function tripet\_index\_offset 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::tripet_index_offset () const
```




<hr>



### function triplet\_count 

```C++
inline auto muda::TripletMatrixViewerBase< IsConst, T, 1 >::triplet_count () const
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::TripletMatrixViewerBase< IsConst, T, 1 >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_indices 

```C++
auto_const_t<int>* muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_col_indices;
```




<hr>



### variable m\_row\_indices 

```C++
auto_const_t<int>* muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_row_indices;
```




<hr>



### variable m\_submatrix\_extent 

```C++
int2 muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_submatrix_extent;
```




<hr>



### variable m\_submatrix\_offset 

```C++
int2 muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_submatrix_offset;
```




<hr>



### variable m\_total\_cols 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_total_cols;
```




<hr>



### variable m\_total\_rows 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_total_rows;
```




<hr>



### variable m\_total\_triplet\_count 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_total_triplet_count;
```




<hr>



### variable m\_triplet\_count 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_triplet_count;
```




<hr>



### variable m\_triplet\_index\_offset 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_triplet_index_offset;
```




<hr>



### variable m\_values 

```C++
auto_const_t<T>* muda::TripletMatrixViewerBase< IsConst, T, 1 >::m_values;
```




<hr>
## Protected Functions Documentation




### function check\_in\_submatrix 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::TripletMatrixViewerBase< IsConst, T, 1 >::check_in_submatrix (
    int i,
    int j
) noexcept const
```




<hr>



### function get\_index 

```C++
inline MUDA_INLINE MUDA_GENERIC int muda::TripletMatrixViewerBase< IsConst, T, 1 >::get_index (
    int i
) noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/triplet_matrix_viewer.h`

