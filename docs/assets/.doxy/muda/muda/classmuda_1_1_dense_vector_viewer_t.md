

# Class muda::DenseVectorViewerT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseVectorViewerT**](classmuda_1_1_dense_vector_viewer_t.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef BufferView&lt; T &gt; | [**BufferView**](#typedef-bufferview)  <br> |
| typedef CBufferView&lt; T &gt; | [**CBufferView**](#typedef-cbufferview)  <br> |
| typedef MapVectorT&lt; const VectorType &gt; | [**CMapVector**](#typedef-cmapvector)  <br> |
| typedef [**DenseVectorViewerT**](classmuda_1_1_dense_vector_viewer_t.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef MapVectorT&lt; VectorType &gt; | [**MapVector**](#typedef-mapvector)  <br> |
| typedef Eigen::Map&lt; U, Eigen::AlignmentType::Unaligned, Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; &gt; | [**MapVectorT**](#typedef-mapvectort)  <br> |
| typedef [**DenseVectorViewerT**](classmuda_1_1_dense_vector_viewer_t.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBufferView, BufferView &gt; | [**ThisBufferView**](#typedef-thisbufferview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CMapVector, MapVector &gt; | [**ThisMapVector**](#typedef-thismapvector)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_vector_viewer_t.md), [**NonConstViewer**](classmuda_1_1_dense_vector_viewer_t.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef Eigen::Vector&lt; T, Eigen::Dynamic &gt; | [**VectorType**](#typedef-vectortype)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseVectorViewerT**](#function-densevectorviewert-23) (auto\_const\_t&lt; T &gt; \* data, int offset, int size, int origin\_size) <br> |
|  MUDA\_GENERIC | [**DenseVectorViewerT**](#function-densevectorviewert-33) (const [**DenseVectorViewerT**](classmuda_1_1_dense_vector_viewer_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|   | [**MUDA\_VIEWER\_COMMON\_NAME**](#function-muda_viewer_common_name) ([**DenseVectorViewerT**](classmuda_1_1_dense_vector_viewer_t.md)) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC Eigen::VectorBlock&lt; ThisMapVector &gt; | [**as\_eigen**](#function-as_eigen) () const<br> |
|  MUDA\_DEVICE T | [**atomic\_add**](#function-atomic_add-13) (int i, T val) const<br> |
|  MUDA\_DEVICE Eigen::Vector&lt; T, N &gt; | [**atomic\_add**](#function-atomic_add-23) (const Eigen::Vector&lt; T, N &gt; & val) const<br> |
|  MUDA\_DEVICE T | [**atomic\_add**](#function-atomic_add-33) (const T & val) <br> |
|  MUDA\_GENERIC auto | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC | [**VectorBlock&lt; ThisMapVector &gt;**](#function-vectorblock<-thismapvector->) () <br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()) (int i) const<br> |
|  MUDA\_GENERIC [**DenseVectorViewerT**](classmuda_1_1_dense_vector_viewer_t.md) & | [**operator=**](#function-operator) (const Eigen::Vector&lt; T, N &gt; & other) <br> |
|  MUDA\_GENERIC auto | [**origin\_data**](#function-origin_data) () const<br> |
|  MUDA\_GENERIC auto | [**origin\_size**](#function-origin_size) () const<br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-12) (int offset, int size) const<br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-22) (int offset) const<br> |
|  MUDA\_GENERIC auto | [**size**](#function-size) () const<br> |


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
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)  <br> |
|  int | [**m\_offset**](#variable-m_offset)   = = 0<br> |
|  int | [**m\_origin\_size**](#variable-m_origin_size)   = = 0<br> |
|  int | [**m\_size**](#variable-m_size)   = = 0<br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_data**](#function-check_data) () const<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_segment**](#function-check_segment) (int offset, int size) const<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_size\_matching**](#function-check_size_matching) (int N) const<br> |
|  MUDA\_INLINE MUDA\_GENERIC int | [**index**](#function-index) (int i) const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef BufferView 

```C++
using muda::DenseVectorViewerT< IsConst, T >::BufferView =  BufferView<T>;
```




<hr>



### typedef CBufferView 

```C++
using muda::DenseVectorViewerT< IsConst, T >::CBufferView =  CBufferView<T>;
```




<hr>



### typedef CMapVector 

```C++
using muda::DenseVectorViewerT< IsConst, T >::CMapVector =  MapVectorT<const VectorType>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DenseVectorViewerT< IsConst, T >::ConstViewer =  DenseVectorViewerT<true, T>;
```




<hr>



### typedef MapVector 

```C++
using muda::DenseVectorViewerT< IsConst, T >::MapVector =  MapVectorT<VectorType>;
```




<hr>



### typedef MapVectorT 

```C++
using muda::DenseVectorViewerT< IsConst, T >::MapVectorT = 
        Eigen::Map<U, Eigen::AlignmentType::Unaligned, Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic>>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DenseVectorViewerT< IsConst, T >::NonConstViewer =  DenseVectorViewerT<false, T>;
```




<hr>



### typedef ThisBufferView 

```C++
using muda::DenseVectorViewerT< IsConst, T >::ThisBufferView =  std::conditional_t<IsConst, CBufferView, BufferView>;
```




<hr>



### typedef ThisMapVector 

```C++
using muda::DenseVectorViewerT< IsConst, T >::ThisMapVector =  std::conditional_t<IsConst, CMapVector, MapVector>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseVectorViewerT< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>



### typedef VectorType 

```C++
using muda::DenseVectorViewerT< IsConst, T >::VectorType =  Eigen::Vector<T, Eigen::Dynamic>;
```




<hr>
## Public Functions Documentation




### function DenseVectorViewerT [2/3]

```C++
inline MUDA_GENERIC muda::DenseVectorViewerT::DenseVectorViewerT (
    auto_const_t< T > * data,
    int offset,
    int size,
    int origin_size
) 
```




<hr>



### function DenseVectorViewerT [3/3]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::DenseVectorViewerT::DenseVectorViewerT (
    const DenseVectorViewerT < OtherIsConst, T > & other
) 
```




<hr>



### function MUDA\_VIEWER\_COMMON\_NAME 

```C++
muda::DenseVectorViewerT::MUDA_VIEWER_COMMON_NAME (
    DenseVectorViewerT
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerT::as_const () const
```




<hr>



### function as\_eigen 

```C++
inline MUDA_GENERIC Eigen::VectorBlock< ThisMapVector > muda::DenseVectorViewerT::as_eigen () const
```




<hr>



### function atomic\_add [1/3]

```C++
inline MUDA_DEVICE T muda::DenseVectorViewerT::atomic_add (
    int i,
    T val
) const
```




<hr>



### function atomic\_add [2/3]

```C++
template<int N>
inline MUDA_DEVICE Eigen::Vector< T, N > muda::DenseVectorViewerT::atomic_add (
    const Eigen::Vector< T, N > & val
) const
```




<hr>



### function atomic\_add [3/3]

```C++
inline MUDA_DEVICE T muda::DenseVectorViewerT::atomic_add (
    const T & val
) 
```




<hr>



### function offset 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerT::offset () const
```




<hr>



### function VectorBlock&lt; ThisMapVector &gt; 

```C++
inline MUDA_GENERIC muda::DenseVectorViewerT::VectorBlock< ThisMapVector > () 
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::DenseVectorViewerT::operator() (
    int i
) const
```




<hr>



### function operator= 

```C++
template<int N>
inline MUDA_GENERIC DenseVectorViewerT & muda::DenseVectorViewerT::operator= (
    const Eigen::Vector< T, N > & other
) 
```




<hr>



### function origin\_data 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerT::origin_data () const
```




<hr>



### function origin\_size 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerT::origin_size () const
```




<hr>



### function segment [1/2]

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerT::segment (
    int offset,
    int size
) const
```




<hr>



### function segment [2/2]

```C++
template<int N>
inline MUDA_GENERIC auto muda::DenseVectorViewerT::segment (
    int offset
) const
```




<hr>



### function size 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerT::size () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::DenseVectorViewerT< IsConst, T >::m_data;
```




<hr>



### variable m\_offset 

```C++
int muda::DenseVectorViewerT< IsConst, T >::m_offset;
```




<hr>



### variable m\_origin\_size 

```C++
int muda::DenseVectorViewerT< IsConst, T >::m_origin_size;
```




<hr>



### variable m\_size 

```C++
int muda::DenseVectorViewerT< IsConst, T >::m_size;
```




<hr>
## Protected Functions Documentation




### function check\_data 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseVectorViewerT::check_data () const
```




<hr>



### function check\_segment 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseVectorViewerT::check_segment (
    int offset,
    int size
) const
```




<hr>



### function check\_size\_matching 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseVectorViewerT::check_size_matching (
    int N
) const
```




<hr>



### function index 

```C++
inline MUDA_INLINE MUDA_GENERIC int muda::DenseVectorViewerT::index (
    int i
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_vector_viewer.h`

