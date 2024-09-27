

# Class muda::DenseVectorViewer

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseVectorViewer**](classmuda_1_1_dense_vector_viewer.md)








Inherits the following classes: [muda::DenseVectorViewerBase](classmuda_1_1_dense_vector_viewer_base.md)
















## Public Types inherited from muda::DenseVectorViewerBase

See [muda::DenseVectorViewerBase](classmuda_1_1_dense_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef BufferView&lt; T &gt; | [**BufferView**](classmuda_1_1_dense_vector_viewer_base.md#typedef-bufferview)  <br> |
| typedef CBufferView&lt; T &gt; | [**CBufferView**](classmuda_1_1_dense_vector_viewer_base.md#typedef-cbufferview)  <br> |
| typedef MapVectorT&lt; const VectorType &gt; | [**CMapVector**](classmuda_1_1_dense_vector_viewer_base.md#typedef-cmapvector)  <br> |
| typedef [**DenseVectorViewerBase**](classmuda_1_1_dense_vector_viewer_base.md)&lt; true, T &gt; | [**ConstViewer**](classmuda_1_1_dense_vector_viewer_base.md#typedef-constviewer)  <br> |
| typedef MapVectorT&lt; VectorType &gt; | [**MapVector**](classmuda_1_1_dense_vector_viewer_base.md#typedef-mapvector)  <br> |
| typedef Eigen::Map&lt; U, Eigen::AlignmentType::Unaligned, Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; &gt; | [**MapVectorT**](classmuda_1_1_dense_vector_viewer_base.md#typedef-mapvectort)  <br> |
| typedef [**DenseVectorViewerBase**](classmuda_1_1_dense_vector_viewer_base.md)&lt; false, T &gt; | [**NonConstViewer**](classmuda_1_1_dense_vector_viewer_base.md#typedef-nonconstviewer)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBufferView, BufferView &gt; | [**ThisBufferView**](classmuda_1_1_dense_vector_viewer_base.md#typedef-thisbufferview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CMapVector, MapVector &gt; | [**ThisMapVector**](classmuda_1_1_dense_vector_viewer_base.md#typedef-thismapvector)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_vector_viewer_base.md), [**NonConstViewer**](classmuda_1_1_dense_vector_viewer_base.md) &gt; | [**ThisViewer**](classmuda_1_1_dense_vector_viewer_base.md#typedef-thisviewer)  <br> |
| typedef Eigen::Vector&lt; T, Eigen::Dynamic &gt; | [**VectorType**](classmuda_1_1_dense_vector_viewer_base.md#typedef-vectortype)  <br> |




















## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseVectorViewer**](#function-densevectorviewer) (const [**Base**](classmuda_1_1_dense_vector_viewer_base.md) & base) <br> |
|  MUDA\_DEVICE T | [**atomic\_add**](#function-atomic_add-13) (int i, T val) <br> |
|  MUDA\_DEVICE Eigen::Vector&lt; T, N &gt; | [**atomic\_add**](#function-atomic_add-23) (const Eigen::Vector&lt; T, N &gt; & val) <br> |
|  MUDA\_DEVICE T | [**atomic\_add**](#function-atomic_add-33) (const T & val) <br> |
|  MUDA\_GENERIC [**DenseVectorViewer**](classmuda_1_1_dense_vector_viewer.md) & | [**operator=**](#function-operator) (const Eigen::Vector&lt; T, N &gt; & other) <br> |
|  MUDA\_GENERIC [**DenseVectorViewer**](classmuda_1_1_dense_vector_viewer.md) | [**segment**](#function-segment-12) (int offset, int size) <br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-22) (int offset) <br> |


## Public Functions inherited from muda::DenseVectorViewerBase

See [muda::DenseVectorViewerBase](classmuda_1_1_dense_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseVectorViewerBase**](classmuda_1_1_dense_vector_viewer_base.md#function-densevectorviewerbase) (auto\_const\_t&lt; T &gt; \* data, int offset, int size, int origin\_size) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](classmuda_1_1_dense_vector_viewer_base.md#function-as_const) () const<br> |
|  MUDA\_GENERIC Eigen::VectorBlock&lt; CMapVector &gt; | [**as\_eigen**](classmuda_1_1_dense_vector_viewer_base.md#function-as_eigen-12) () const<br> |
|  MUDA\_GENERIC Eigen::VectorBlock&lt; ThisMapVector &gt; | [**as\_eigen**](classmuda_1_1_dense_vector_viewer_base.md#function-as_eigen-22) () <br> |
|  MUDA\_GENERIC auto | [**offset**](classmuda_1_1_dense_vector_viewer_base.md#function-offset) () const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](classmuda_1_1_dense_vector_viewer_base.md#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC | [**VectorBlock&lt; CMapVector &gt;**](classmuda_1_1_dense_vector_viewer_base.md#function-vectorblock<-cmapvector->) () const<br> |
|  MUDA\_GENERIC | [**VectorBlock&lt; ThisMapVector &gt;**](classmuda_1_1_dense_vector_viewer_base.md#function-vectorblock<-thismapvector->) () <br> |
|  MUDA\_GENERIC const T & | [**operator()**](classmuda_1_1_dense_vector_viewer_base.md#function-operator()-12) (int i) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](classmuda_1_1_dense_vector_viewer_base.md#function-operator()-22) (int i) <br> |
|  MUDA\_GENERIC auto | [**origin\_data**](classmuda_1_1_dense_vector_viewer_base.md#function-origin_data) () const<br> |
|  MUDA\_GENERIC auto | [**origin\_size**](classmuda_1_1_dense_vector_viewer_base.md#function-origin_size) () const<br> |
|  MUDA\_GENERIC auto | [**segment**](classmuda_1_1_dense_vector_viewer_base.md#function-segment-14) (int offset, int size) <br> |
|  MUDA\_GENERIC auto | [**segment**](classmuda_1_1_dense_vector_viewer_base.md#function-segment-24) (int offset) <br> |
|  MUDA\_GENERIC auto | [**segment**](classmuda_1_1_dense_vector_viewer_base.md#function-segment-34) (int offset, int size) const<br> |
|  MUDA\_GENERIC auto | [**segment**](classmuda_1_1_dense_vector_viewer_base.md#function-segment-44) (int offset) const<br> |
|  MUDA\_GENERIC auto | [**size**](classmuda_1_1_dense_vector_viewer_base.md#function-size) () const<br> |


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










## Protected Attributes inherited from muda::DenseVectorViewerBase

See [muda::DenseVectorViewerBase](classmuda_1_1_dense_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](classmuda_1_1_dense_vector_viewer_base.md#variable-m_data)  <br> |
|  int | [**m\_offset**](classmuda_1_1_dense_vector_viewer_base.md#variable-m_offset)   = = 0<br> |
|  int | [**m\_origin\_size**](classmuda_1_1_dense_vector_viewer_base.md#variable-m_origin_size)   = = 0<br> |
|  int | [**m\_size**](classmuda_1_1_dense_vector_viewer_base.md#variable-m_size)   = = 0<br> |
















































## Protected Functions inherited from muda::DenseVectorViewerBase

See [muda::DenseVectorViewerBase](classmuda_1_1_dense_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_data**](classmuda_1_1_dense_vector_viewer_base.md#function-check_data) () const<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_segment**](classmuda_1_1_dense_vector_viewer_base.md#function-check_segment) (int offset, int size) const<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_size\_matching**](classmuda_1_1_dense_vector_viewer_base.md#function-check_size_matching) (int N) <br> |
|  MUDA\_INLINE MUDA\_GENERIC int | [**index**](classmuda_1_1_dense_vector_viewer_base.md#function-index) (int i) const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |








## Public Functions Documentation




### function DenseVectorViewer 

```C++
inline MUDA_GENERIC muda::DenseVectorViewer::DenseVectorViewer (
    const Base & base
) 
```




<hr>



### function atomic\_add [1/3]

```C++
inline MUDA_DEVICE T muda::DenseVectorViewer::atomic_add (
    int i,
    T val
) 
```




<hr>



### function atomic\_add [2/3]

```C++
template<int N>
inline MUDA_DEVICE Eigen::Vector< T, N > muda::DenseVectorViewer::atomic_add (
    const Eigen::Vector< T, N > & val
) 
```




<hr>



### function atomic\_add [3/3]

```C++
inline MUDA_DEVICE T muda::DenseVectorViewer::atomic_add (
    const T & val
) 
```




<hr>



### function operator= 

```C++
template<int N>
inline MUDA_GENERIC DenseVectorViewer & muda::DenseVectorViewer::operator= (
    const Eigen::Vector< T, N > & other
) 
```




<hr>



### function segment [1/2]

```C++
inline MUDA_GENERIC DenseVectorViewer muda::DenseVectorViewer::segment (
    int offset,
    int size
) 
```




<hr>



### function segment [2/2]

```C++
template<int N>
inline MUDA_GENERIC auto muda::DenseVectorViewer::segment (
    int offset
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_vector_viewer.h`

