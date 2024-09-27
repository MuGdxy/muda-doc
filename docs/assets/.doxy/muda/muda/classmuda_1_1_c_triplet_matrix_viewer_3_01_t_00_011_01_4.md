

# Class muda::CTripletMatrixViewer&lt; T, 1 &gt;

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**CTripletMatrixViewer&lt; T, 1 &gt;**](classmuda_1_1_c_triplet_matrix_viewer_3_01_t_00_011_01_4.md)








Inherits the following classes: [muda::TripletMatrixViewerBase](classmuda_1_1_triplet_matrix_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**CTripletMatrixViewer**](classmuda_1_1_c_triplet_matrix_viewer.md)&lt; T, 1 &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |


## Public Types inherited from muda::TripletMatrixViewerBase

See [muda::TripletMatrixViewerBase](classmuda_1_1_triplet_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; T, N, N &gt; | [**BlockMatrix**](classmuda_1_1_triplet_matrix_viewer_base.md#typedef-blockmatrix)  <br> |
| typedef [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md)&lt; true, T, N &gt; | [**ConstViewer**](classmuda_1_1_triplet_matrix_viewer_base.md#typedef-constviewer)  <br> |
| typedef [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md)&lt; false, T, N &gt; | [**NonConstViewer**](classmuda_1_1_triplet_matrix_viewer_base.md#typedef-nonconstviewer)  <br> |
| typedef [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md)&lt; IsConst, T, N &gt; | [**ThisViewer**](classmuda_1_1_triplet_matrix_viewer_base.md#typedef-thisviewer)  <br> |




















## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**CTripletMatrixViewer**](#function-ctripletmatrixviewer) (const [**Base**](classmuda_1_1_triplet_matrix_viewer_base.md) & base) <br> |


## Public Functions inherited from muda::TripletMatrixViewerBase

See [muda::TripletMatrixViewerBase](classmuda_1_1_triplet_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md#function-tripletmatrixviewerbase-12) () = default<br> |
|  MUDA\_GENERIC | [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md#function-tripletmatrixviewerbase-22) (int total\_block\_rows, int total\_block\_cols, int triplet\_index\_offset, int triplet\_count, int total\_triplet\_count, int2 submatrix\_offset, int2 submatrix\_extent, auto\_const\_t&lt; int &gt; \* block\_row\_indices, auto\_const\_t&lt; int &gt; \* block\_col\_indices, auto\_const\_t&lt; BlockMatrix &gt; \* block\_values) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_triplet_matrix_viewer_base.md) | [**as\_const**](classmuda_1_1_triplet_matrix_viewer_base.md#function-as_const) () const<br> |
|  MUDA\_GENERIC auto | [**extent**](classmuda_1_1_triplet_matrix_viewer_base.md#function-extent) () const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](classmuda_1_1_triplet_matrix_viewer_base.md#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC [**CTriplet**](structmuda_1_1_triplet_matrix_viewer_base_1_1_c_triplet.md) | [**operator()**](classmuda_1_1_triplet_matrix_viewer_base.md#function-operator()) (int i) const<br> |
|  MUDA\_GENERIC auto | [**submatrix\_offset**](classmuda_1_1_triplet_matrix_viewer_base.md#function-submatrix_offset) () const<br> |
|  MUDA\_GENERIC auto | [**total\_block\_cols**](classmuda_1_1_triplet_matrix_viewer_base.md#function-total_block_cols) () const<br> |
|  MUDA\_GENERIC auto | [**total\_block\_rows**](classmuda_1_1_triplet_matrix_viewer_base.md#function-total_block_rows) () const<br> |
|  MUDA\_GENERIC auto | [**total\_extent**](classmuda_1_1_triplet_matrix_viewer_base.md#function-total_extent) () const<br> |
|  MUDA\_GENERIC auto | [**total\_triplet\_count**](classmuda_1_1_triplet_matrix_viewer_base.md#function-total_triplet_count) () const<br> |
|  MUDA\_GENERIC auto | [**tripet\_index\_offset**](classmuda_1_1_triplet_matrix_viewer_base.md#function-tripet_index_offset) () const<br> |
|  MUDA\_GENERIC auto | [**triplet\_count**](classmuda_1_1_triplet_matrix_viewer_base.md#function-triplet_count) () const<br> |


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












## Protected Types inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_viewer_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_viewer_base.md#typedef-non_const_enable_t)  <br> |










## Protected Attributes inherited from muda::TripletMatrixViewerBase

See [muda::TripletMatrixViewerBase](classmuda_1_1_triplet_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; int &gt; \* | [**m\_block\_col\_indices**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_block_col_indices)  <br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_block\_row\_indices**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_block_row_indices)  <br> |
|  auto\_const\_t&lt; BlockMatrix &gt; \* | [**m\_block\_values**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_block_values)  <br> |
|  int2 | [**m\_submatrix\_extent**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_submatrix_extent)   = = {0, 0}<br> |
|  int2 | [**m\_submatrix\_offset**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_submatrix_offset)   = = {0, 0}<br> |
|  int | [**m\_total\_block\_cols**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_total_block_cols)   = = 0<br> |
|  int | [**m\_total\_block\_rows**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_total_block_rows)   = = 0<br> |
|  int | [**m\_total\_triplet\_count**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_total_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_count**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_triplet_count)   = = 0<br> |
|  int | [**m\_triplet\_index\_offset**](classmuda_1_1_triplet_matrix_viewer_base.md#variable-m_triplet_index_offset)   = = 0<br> |
















































## Protected Functions inherited from muda::TripletMatrixViewerBase

See [muda::TripletMatrixViewerBase](classmuda_1_1_triplet_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_in\_submatrix**](classmuda_1_1_triplet_matrix_viewer_base.md#function-check_in_submatrix) (int i, int j) noexcept const<br> |
|  MUDA\_INLINE MUDA\_GENERIC int | [**get\_index**](classmuda_1_1_triplet_matrix_viewer_base.md#function-get_index) (int i) noexcept const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |








## Public Types Documentation




### typedef ConstViewer 

```C++
using muda::CTripletMatrixViewer< T, 1 >::ConstViewer =  CTripletMatrixViewer<T, 1>;
```




<hr>
## Public Functions Documentation




### function CTripletMatrixViewer 

```C++
inline MUDA_GENERIC muda::CTripletMatrixViewer< T, 1 >::CTripletMatrixViewer (
    const Base & base
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/triplet_matrix_viewer.h`

