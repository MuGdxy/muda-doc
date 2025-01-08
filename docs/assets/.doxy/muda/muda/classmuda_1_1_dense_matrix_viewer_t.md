

# Class muda::DenseMatrixViewerT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseMatrixViewerT**](classmuda_1_1_dense_matrix_viewer_t.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Buffer2DView&lt; T &gt; | [**Buffer2DView**](#typedef-buffer2dview)  <br> |
| typedef CBuffer2DView&lt; T &gt; | [**CBuffer2DView**](#typedef-cbuffer2dview)  <br> |
| typedef MapMatrixT&lt; const MatrixType &gt; | [**CMapMatrix**](#typedef-cmapmatrix)  <br> |
| typedef [**DenseMatrixViewerT**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef MapMatrixT&lt; MatrixType &gt; | [**MapMatrix**](#typedef-mapmatrix)  <br> |
| typedef Eigen::Map&lt; U, Eigen::AlignmentType::Unaligned, Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; &gt; | [**MapMatrixT**](#typedef-mapmatrixt)  <br> |
| typedef Eigen::Matrix&lt; T, Eigen::Dynamic, Eigen::Dynamic, Eigen::ColMajor &gt; | [**MatrixType**](#typedef-matrixtype)  <br> |
| typedef [**DenseMatrixViewerT**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBuffer2DView, Buffer2DView &gt; | [**ThisBuffer2DView**](#typedef-thisbuffer2dview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CMapMatrix, MapMatrix &gt; | [**ThisMapMatrix**](#typedef-thismapmatrix)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_matrix_viewer_t.md), [**NonConstViewer**](classmuda_1_1_dense_matrix_viewer_t.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseMatrixViewerT**](#function-densematrixviewert-23) (ThisBuffer2DView view, size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) <br> |
|  MUDA\_GENERIC | [**DenseMatrixViewerT**](#function-densematrixviewert-33) (const [**DenseMatrixViewerT**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|   | [**MUDA\_VIEWER\_COMMON\_NAME**](#function-muda_viewer_common_name) ([**DenseMatrixViewerT**](classmuda_1_1_dense_matrix_viewer_t.md)) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC Eigen::Block&lt; ThisMapMatrix &gt; | [**as\_eigen**](#function-as_eigen) () const<br> |
|  MUDA\_DEVICE T | [**atomic\_add**](#function-atomic_add-12) (size\_t i, size\_t j, T val) const<br> |
|  MUDA\_DEVICE Eigen::Matrix&lt; T, M, N &gt; | [**atomic\_add**](#function-atomic_add-22) (const Eigen::Matrix&lt; T, M, N &gt; & other) const<br> |
|  MUDA\_GENERIC ThisViewer | [**block**](#function-block-12) (size\_t row\_offset, size\_t col\_offset, size\_t row\_size, size\_t col\_size) const<br> |
|  MUDA\_GENERIC ThisViewer | [**block**](#function-block-22) (int row\_offset, int col\_offset) <br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](#function-buffer_view) () const<br> |
|  MUDA\_GENERIC size\_t | [**col**](#function-col) () const<br> |
|  MUDA\_GENERIC auto | [**col\_offset**](#function-col_offset) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()) (size\_t i, size\_t j) const<br> |
|  MUDA\_GENERIC [**DenseMatrixViewerT**](classmuda_1_1_dense_matrix_viewer_t.md) & | [**operator=**](#function-operator) (const Eigen::Matrix&lt; T, M, N &gt; & other) const<br> |
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
using muda::DenseMatrixViewerT< IsConst, T >::Buffer2DView =  Buffer2DView<T>;
```




<hr>



### typedef CBuffer2DView 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::CBuffer2DView =  CBuffer2DView<T>;
```




<hr>



### typedef CMapMatrix 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::CMapMatrix =  MapMatrixT<const MatrixType>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::ConstViewer =  DenseMatrixViewerT<true, T>;
```




<hr>



### typedef MapMatrix 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::MapMatrix =  MapMatrixT<MatrixType>;
```




<hr>



### typedef MapMatrixT 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::MapMatrixT = 
        Eigen::Map<U, Eigen::AlignmentType::Unaligned, Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic>>;
```




<hr>



### typedef MatrixType 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::MatrixType =  Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic, Eigen::ColMajor>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::NonConstViewer =  DenseMatrixViewerT<false, T>;
```




<hr>



### typedef ThisBuffer2DView 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::ThisBuffer2DView =  std::conditional_t<IsConst, CBuffer2DView, Buffer2DView>;
```




<hr>



### typedef ThisMapMatrix 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::ThisMapMatrix =  std::conditional_t<IsConst, CMapMatrix, MapMatrix>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseMatrixViewerT< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>
## Public Functions Documentation




### function DenseMatrixViewerT [2/3]

```C++
inline MUDA_GENERIC muda::DenseMatrixViewerT::DenseMatrixViewerT (
    ThisBuffer2DView view,
    size_t row_offset,
    size_t col_offset,
    size_t row_size,
    size_t col_size
) 
```




<hr>



### function DenseMatrixViewerT [3/3]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::DenseMatrixViewerT::DenseMatrixViewerT (
    const DenseMatrixViewerT < OtherIsConst, T > & other
) 
```




<hr>



### function MUDA\_VIEWER\_COMMON\_NAME 

```C++
muda::DenseMatrixViewerT::MUDA_VIEWER_COMMON_NAME (
    DenseMatrixViewerT
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerT::as_const () const
```




<hr>



### function as\_eigen 

```C++
inline MUDA_GENERIC Eigen::Block< ThisMapMatrix > muda::DenseMatrixViewerT::as_eigen () const
```




<hr>



### function atomic\_add [1/2]

```C++
inline MUDA_DEVICE T muda::DenseMatrixViewerT::atomic_add (
    size_t i,
    size_t j,
    T val
) const
```




<hr>



### function atomic\_add [2/2]

```C++
template<int M, int N>
inline MUDA_DEVICE Eigen::Matrix< T, M, N > muda::DenseMatrixViewerT::atomic_add (
    const Eigen::Matrix< T, M, N > & other
) const
```




<hr>



### function block [1/2]

```C++
inline MUDA_GENERIC ThisViewer muda::DenseMatrixViewerT::block (
    size_t row_offset,
    size_t col_offset,
    size_t row_size,
    size_t col_size
) const
```




<hr>



### function block [2/2]

```C++
template<int M, int N>
inline MUDA_GENERIC ThisViewer muda::DenseMatrixViewerT::block (
    int row_offset,
    int col_offset
) 
```




<hr>



### function buffer\_view 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerT::buffer_view () const
```




<hr>



### function col 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewerT::col () const
```




<hr>



### function col\_offset 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerT::col_offset () const
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::DenseMatrixViewerT::operator() (
    size_t i,
    size_t j
) const
```




<hr>



### function operator= 

```C++
template<int M, int N>
inline MUDA_GENERIC DenseMatrixViewerT & muda::DenseMatrixViewerT::operator= (
    const Eigen::Matrix< T, M, N > & other
) const
```




<hr>



### function origin\_col 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewerT::origin_col () const
```




<hr>



### function origin\_row 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewerT::origin_row () const
```




<hr>



### function row 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewerT::row () const
```




<hr>



### function row\_offset 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewerT::row_offset () const
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_offset 

```C++
size_t muda::DenseMatrixViewerT< IsConst, T >::m_col_offset;
```




<hr>



### variable m\_col\_size 

```C++
size_t muda::DenseMatrixViewerT< IsConst, T >::m_col_size;
```




<hr>



### variable m\_row\_offset 

```C++
size_t muda::DenseMatrixViewerT< IsConst, T >::m_row_offset;
```




<hr>



### variable m\_row\_size 

```C++
size_t muda::DenseMatrixViewerT< IsConst, T >::m_row_size;
```




<hr>



### variable m\_view 

```C++
ThisBuffer2DView muda::DenseMatrixViewerT< IsConst, T >::m_view;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_matrix_viewer.h`

