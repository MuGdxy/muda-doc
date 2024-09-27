

# Class muda::DenseMatrixViewerBase

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseMatrixViewerBase**](classmuda_1_1_dense_matrix_viewer_base.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Buffer2DView&lt; T &gt; | [**Buffer2DView**](#typedef-buffer2dview)  <br> |
| typedef CBuffer2DView&lt; T &gt; | [**CBuffer2DView**](#typedef-cbuffer2dview)  <br> |
| typedef MapMatrixT&lt; const MatrixType &gt; | [**CMapMatrix**](#typedef-cmapmatrix)  <br> |
| typedef [**DenseMatrixViewerBase**](classmuda_1_1_dense_matrix_viewer_base.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef MapMatrixT&lt; MatrixType &gt; | [**MapMatrix**](#typedef-mapmatrix)  <br> |
| typedef Eigen::Map&lt; U, Eigen::AlignmentType::Unaligned, Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; &gt; | [**MapMatrixT**](#typedef-mapmatrixt)  <br> |
| typedef Eigen::Matrix&lt; T, Eigen::Dynamic, Eigen::Dynamic, Eigen::ColMajor &gt; | [**MatrixType**](#typedef-matrixtype)  <br> |
| typedef [**DenseMatrixViewerBase**](classmuda_1_1_dense_matrix_viewer_base.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBuffer2DView, Buffer2DView &gt; | [**ThisBuffer2DView**](#typedef-thisbuffer2dview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CMapMatrix, MapMatrix &gt; | [**ThisMapMatrix**](#typedef-thismapmatrix)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md), [**NonConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseMatrixViewerBase**](#function-densematrixviewerbase) (ThisBuffer2DView view, size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC Eigen::Block&lt; ThisMapMatrix &gt; | [**as\_eigen**](#function-as_eigen-12) () <br> |
|  MUDA\_GENERIC Eigen::Block&lt; CMapMatrix &gt; | [**as\_eigen**](#function-as_eigen-22) () const<br> |
|  MUDA\_GENERIC ThisViewer | [**block**](#function-block-14) (size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) <br> |
|  MUDA\_GENERIC ThisViewer | [**block**](#function-block-24) (int row\_offset, int col\_offset) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md) | [**block**](#function-block-34) (size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) const<br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_base.md) | [**block**](#function-block-44) (int row\_offset, int col\_offset) const<br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](#function-buffer_view-12) () <br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](#function-buffer_view-22) () const<br> |
|  MUDA\_GENERIC size\_t | [**col**](#function-col) () const<br> |
|  MUDA\_GENERIC auto | [**col\_offset**](#function-col_offset) () const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC | [**Block&lt; CMapMatrix &gt;**](#function-block<-cmapmatrix->-12) () <br> |
|  MUDA\_GENERIC | [**Block&lt; CMapMatrix &gt;**](#function-block<-cmapmatrix->-22) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()-12) (size\_t i, size\_t j) <br> |
|  MUDA\_GENERIC const T & | [**operator()**](#function-operator()-22) (size\_t i, size\_t j) const<br> |
|  MUDA\_GENERIC size\_t | [**origin\_col**](#function-origin_col) () const<br> |
|  MUDA\_GENERIC size\_t | [**origin\_row**](#function-origin_row) () const<br> |
|  MUDA\_GENERIC size\_t | [**row**](#function-row) () const<br> |
|  MUDA\_GENERIC auto | [**row\_offset**](#function-row_offset) () const<br> |


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






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  size\_t | [**m\_col\_offset**](#variable-m_col_offset)   = = 0<br> |
|  size\_t | [**m\_col\_size**](#variable-m_col_size)   = = 0<br> |
|  size\_t | [**m\_row\_offset**](#variable-m_row_offset)   = = 0<br> |
|  size\_t | [**m\_row\_size**](#variable-m_row_size)   = = 0<br> |
|  ThisBuffer2DView | [**m\_view**](#variable-m_view)  <br> |


































## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef Buffer2DView 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::Buffer2DView =  Buffer2DView<T>;
```




<hr>



### typedef CBuffer2DView 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::CBuffer2DView =  CBuffer2DView<T>;
```




<hr>



### typedef CMapMatrix 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::CMapMatrix =  MapMatrixT<const MatrixType>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::ConstViewer =  DenseMatrixViewerBase<true, T>;
```




<hr>



### typedef MapMatrix 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::MapMatrix =  MapMatrixT<MatrixType>;
```




<hr>



### typedef MapMatrixT 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::MapMatrixT =  Eigen::Map<U, Eigen::AlignmentType::Unaligned, Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic> >;
```




<hr>



### typedef MatrixType 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::MatrixType =  Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic, Eigen::ColMajor>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::NonConstViewer =  DenseMatrixViewerBase<false, T>;
```




<hr>



### typedef ThisBuffer2DView 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::ThisBuffer2DView =  std::conditional_t<IsConst, CBuffer2DView, Buffer2DView>;
```




<hr>



### typedef ThisMapMatrix 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::ThisMapMatrix =  std::conditional_t<IsConst, CMapMatrix, MapMatrix>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseMatrixViewerBase< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>
## Public Functions Documentation




### function DenseMatrixViewerBase 

```C++
inline MUDA_GENERIC muda::DenseMatrixViewerBase::DenseMatrixViewerBase (
    ThisBuffer2DView view,
    size_t row_offset,
    size_t col_offset,
    size_t row_size,
    size_t col_size
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerBase::as_const () const
```




<hr>



### function as\_eigen [1/2]

```C++
MUDA_GENERIC Eigen::Block< ThisMapMatrix > muda::DenseMatrixViewerBase::as_eigen () 
```




<hr>



### function as\_eigen [2/2]

```C++
MUDA_GENERIC Eigen::Block< CMapMatrix > muda::DenseMatrixViewerBase::as_eigen () const
```




<hr>



### function block [1/4]

```C++
MUDA_GENERIC ThisViewer muda::DenseMatrixViewerBase::block (
    size_t row_offset,
    size_t col_offset,
    size_t row_size,
    size_t col_size
) 
```




<hr>



### function block [2/4]

```C++
template<int M, int N>
inline MUDA_GENERIC ThisViewer muda::DenseMatrixViewerBase::block (
    int row_offset,
    int col_offset
) 
```




<hr>



### function block [3/4]

```C++
inline MUDA_GENERIC ConstViewer muda::DenseMatrixViewerBase::block (
    size_t row_offset,
    size_t col_offset,
    size_t row_size,
    size_t col_size
) const
```




<hr>



### function block [4/4]

```C++
template<int M, int N>
inline MUDA_GENERIC ConstViewer muda::DenseMatrixViewerBase::block (
    int row_offset,
    int col_offset
) const
```




<hr>



### function buffer\_view [1/2]

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerBase::buffer_view () 
```




<hr>



### function buffer\_view [2/2]

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerBase::buffer_view () const
```




<hr>



### function col 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewerBase::col () const
```




<hr>



### function col\_offset 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerBase::col_offset () const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::DenseMatrixViewerBase::operator ConstViewer () const
```




<hr>



### function Block&lt; CMapMatrix &gt; [1/2]

```C++
MUDA_GENERIC muda::DenseMatrixViewerBase::Block< CMapMatrix > () 
```




<hr>



### function Block&lt; CMapMatrix &gt; [2/2]

```C++
inline MUDA_GENERIC muda::DenseMatrixViewerBase::Block< CMapMatrix > () const
```




<hr>



### function operator() [1/2]

```C++
MUDA_GENERIC auto_const_t< T > & muda::DenseMatrixViewerBase::operator() (
    size_t i,
    size_t j
) 
```




<hr>



### function operator() [2/2]

```C++
inline MUDA_GENERIC const T & muda::DenseMatrixViewerBase::operator() (
    size_t i,
    size_t j
) const
```




<hr>



### function origin\_col 

```C++
MUDA_GENERIC size_t muda::DenseMatrixViewerBase::origin_col () const
```




<hr>



### function origin\_row 

```C++
MUDA_GENERIC size_t muda::DenseMatrixViewerBase::origin_row () const
```




<hr>



### function row 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewerBase::row () const
```




<hr>



### function row\_offset 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerBase::row_offset () const
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_offset 

```C++
size_t muda::DenseMatrixViewerBase< IsConst, T >::m_col_offset;
```




<hr>



### variable m\_col\_size 

```C++
size_t muda::DenseMatrixViewerBase< IsConst, T >::m_col_size;
```




<hr>



### variable m\_row\_offset 

```C++
size_t muda::DenseMatrixViewerBase< IsConst, T >::m_row_offset;
```




<hr>



### variable m\_row\_size 

```C++
size_t muda::DenseMatrixViewerBase< IsConst, T >::m_row_size;
```




<hr>



### variable m\_view 

```C++
ThisBuffer2DView muda::DenseMatrixViewerBase< IsConst, T >::m_view;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_matrix_viewer.h`

