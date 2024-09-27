

# Class muda::DenseMatrixViewer

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer.md)








Inherits the following classes: [muda::DenseMatrixViewerBase](classmuda_1_1_dense_matrix_viewer_base.md)
















## Public Types inherited from muda::DenseMatrixViewerBase

See [muda::DenseMatrixViewerBase](classmuda_1_1_dense_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef Buffer2DView&lt; T &gt; | [**Buffer2DView**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-buffer2dview)  <br> |
| typedef CBuffer2DView&lt; T &gt; | [**CBuffer2DView**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-cbuffer2dview)  <br> |
| typedef MapMatrixT&lt; const MatrixType &gt; | [**CMapMatrix**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-cmapmatrix)  <br> |
| typedef [**DenseMatrixViewerBase**](classmuda_1_1_dense_matrix_viewer_base.md)&lt; true, T &gt; | [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-constviewer)  <br> |
| typedef MapMatrixT&lt; MatrixType &gt; | [**MapMatrix**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-mapmatrix)  <br> |
| typedef Eigen::Map&lt; U, Eigen::AlignmentType::Unaligned, Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; &gt; | [**MapMatrixT**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-mapmatrixt)  <br> |
| typedef Eigen::Matrix&lt; T, Eigen::Dynamic, Eigen::Dynamic, Eigen::ColMajor &gt; | [**MatrixType**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-matrixtype)  <br> |
| typedef [**DenseMatrixViewerBase**](classmuda_1_1_dense_matrix_viewer_base.md)&lt; false, T &gt; | [**NonConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-nonconstviewer)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBuffer2DView, Buffer2DView &gt; | [**ThisBuffer2DView**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-thisbuffer2dview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CMapMatrix, MapMatrix &gt; | [**ThisMapMatrix**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-thismapmatrix)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md), [**NonConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md) &gt; | [**ThisViewer**](classmuda_1_1_dense_matrix_viewer_base.md#typedef-thisviewer)  <br> |




















## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseMatrixViewer**](#function-densematrixviewer-12) (const [**Base**](classmuda_1_1_dense_matrix_viewer_base.md) & base) <br> |
|  MUDA\_GENERIC | [**DenseMatrixViewer**](#function-densematrixviewer-22) (const [**CDenseMatrixViewer**](classmuda_1_1_c_dense_matrix_viewer.md)&lt; T &gt; &) = delete<br> |
|  MUDA\_DEVICE T | [**atomic\_add**](#function-atomic_add-12) (size\_t i, size\_t j, T val) <br> |
|  MUDA\_DEVICE Eigen::Matrix&lt; T, M, N &gt; | [**atomic\_add**](#function-atomic_add-22) (const Eigen::Matrix&lt; T, M, N &gt; & other) <br> |
|  MUDA\_GENERIC [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer.md) | [**block**](#function-block-12) (size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) <br> |
|  MUDA\_GENERIC [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer.md) | [**block**](#function-block-22) (size\_t row\_offset, size\_t col\_offset) <br> |
|  MUDA\_GENERIC [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer.md) & | [**operator=**](#function-operator) (const Eigen::Matrix&lt; T, M, N &gt; & other) <br> |


## Public Functions inherited from muda::DenseMatrixViewerBase

See [muda::DenseMatrixViewerBase](classmuda_1_1_dense_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseMatrixViewerBase**](classmuda_1_1_dense_matrix_viewer_base.md#function-densematrixviewerbase) (ThisBuffer2DView view, size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](classmuda_1_1_dense_matrix_viewer_base.md#function-as_const) () const<br> |
|  MUDA\_GENERIC Eigen::Block&lt; ThisMapMatrix &gt; | [**as\_eigen**](classmuda_1_1_dense_matrix_viewer_base.md#function-as_eigen-12) () <br> |
|  MUDA\_GENERIC Eigen::Block&lt; CMapMatrix &gt; | [**as\_eigen**](classmuda_1_1_dense_matrix_viewer_base.md#function-as_eigen-22) () const<br> |
|  MUDA\_GENERIC ThisViewer | [**block**](classmuda_1_1_dense_matrix_viewer_base.md#function-block-14) (size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) <br> |
|  MUDA\_GENERIC ThisViewer | [**block**](classmuda_1_1_dense_matrix_viewer_base.md#function-block-24) (int row\_offset, int col\_offset) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md) | [**block**](classmuda_1_1_dense_matrix_viewer_base.md#function-block-34) (size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) const<br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md) | [**block**](classmuda_1_1_dense_matrix_viewer_base.md#function-block-44) (int row\_offset, int col\_offset) const<br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](classmuda_1_1_dense_matrix_viewer_base.md#function-buffer_view-12) () <br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](classmuda_1_1_dense_matrix_viewer_base.md#function-buffer_view-22) () const<br> |
|  MUDA\_GENERIC size\_t | [**col**](classmuda_1_1_dense_matrix_viewer_base.md#function-col) () const<br> |
|  MUDA\_GENERIC auto | [**col\_offset**](classmuda_1_1_dense_matrix_viewer_base.md#function-col_offset) () const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC | [**Block&lt; CMapMatrix &gt;**](classmuda_1_1_dense_matrix_viewer_base.md#function-block<-cmapmatrix->-12) () <br> |
|  MUDA\_GENERIC | [**Block&lt; CMapMatrix &gt;**](classmuda_1_1_dense_matrix_viewer_base.md#function-block<-cmapmatrix->-22) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](classmuda_1_1_dense_matrix_viewer_base.md#function-operator()-12) (size\_t i, size\_t j) <br> |
|  MUDA\_GENERIC const T & | [**operator()**](classmuda_1_1_dense_matrix_viewer_base.md#function-operator()-22) (size\_t i, size\_t j) const<br> |
|  MUDA\_GENERIC size\_t | [**origin\_col**](classmuda_1_1_dense_matrix_viewer_base.md#function-origin_col) () const<br> |
|  MUDA\_GENERIC size\_t | [**origin\_row**](classmuda_1_1_dense_matrix_viewer_base.md#function-origin_row) () const<br> |
|  MUDA\_GENERIC size\_t | [**row**](classmuda_1_1_dense_matrix_viewer_base.md#function-row) () const<br> |
|  MUDA\_GENERIC auto | [**row\_offset**](classmuda_1_1_dense_matrix_viewer_base.md#function-row_offset) () const<br> |


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










## Protected Attributes inherited from muda::DenseMatrixViewerBase

See [muda::DenseMatrixViewerBase](classmuda_1_1_dense_matrix_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  size\_t | [**m\_col\_offset**](classmuda_1_1_dense_matrix_viewer_base.md#variable-m_col_offset)   = = 0<br> |
|  size\_t | [**m\_col\_size**](classmuda_1_1_dense_matrix_viewer_base.md#variable-m_col_size)   = = 0<br> |
|  size\_t | [**m\_row\_offset**](classmuda_1_1_dense_matrix_viewer_base.md#variable-m_row_offset)   = = 0<br> |
|  size\_t | [**m\_row\_size**](classmuda_1_1_dense_matrix_viewer_base.md#variable-m_row_size)   = = 0<br> |
|  ThisBuffer2DView | [**m\_view**](classmuda_1_1_dense_matrix_viewer_base.md#variable-m_view)  <br> |


















































## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |








## Public Functions Documentation




### function DenseMatrixViewer [1/2]

```C++
inline MUDA_GENERIC muda::DenseMatrixViewer::DenseMatrixViewer (
    const Base & base
) 
```




<hr>



### function DenseMatrixViewer [2/2]

```C++
MUDA_GENERIC muda::DenseMatrixViewer::DenseMatrixViewer (
    const CDenseMatrixViewer < T > &
) = delete
```




<hr>



### function atomic\_add [1/2]

```C++
MUDA_DEVICE T muda::DenseMatrixViewer::atomic_add (
    size_t i,
    size_t j,
    T val
) 
```




<hr>



### function atomic\_add [2/2]

```C++
template<int M, int N>
MUDA_DEVICE Eigen::Matrix< T, M, N > muda::DenseMatrixViewer::atomic_add (
    const Eigen::Matrix< T, M, N > & other
) 
```




<hr>



### function block [1/2]

```C++
inline MUDA_GENERIC DenseMatrixViewer muda::DenseMatrixViewer::block (
    size_t row_offset,
    size_t col_offset,
    size_t row_size,
    size_t col_size
) 
```




<hr>



### function block [2/2]

```C++
template<size_t M, size_t N>
inline MUDA_GENERIC DenseMatrixViewer muda::DenseMatrixViewer::block (
    size_t row_offset,
    size_t col_offset
) 
```




<hr>



### function operator= 

```C++
template<int M, int N>
MUDA_GENERIC DenseMatrixViewer & muda::DenseMatrixViewer::operator= (
    const Eigen::Matrix< T, M, N > & other
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_matrix_viewer.h`

