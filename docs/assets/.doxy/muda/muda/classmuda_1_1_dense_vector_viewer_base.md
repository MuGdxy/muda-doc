

# Class muda::DenseVectorViewerBase

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseVectorViewerBase**](classmuda_1_1_dense_vector_viewer_base.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef BufferView&lt; T &gt; | [**BufferView**](#typedef-bufferview)  <br> |
| typedef CBufferView&lt; T &gt; | [**CBufferView**](#typedef-cbufferview)  <br> |
| typedef MapVectorT&lt; const VectorType &gt; | [**CMapVector**](#typedef-cmapvector)  <br> |
| typedef [**DenseVectorViewerBase**](classmuda_1_1_dense_vector_viewer_base.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef MapVectorT&lt; VectorType &gt; | [**MapVector**](#typedef-mapvector)  <br> |
| typedef Eigen::Map&lt; U, Eigen::AlignmentType::Unaligned, Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; &gt; | [**MapVectorT**](#typedef-mapvectort)  <br> |
| typedef [**DenseVectorViewerBase**](classmuda_1_1_dense_vector_viewer_base.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBufferView, BufferView &gt; | [**ThisBufferView**](#typedef-thisbufferview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CMapVector, MapVector &gt; | [**ThisMapVector**](#typedef-thismapvector)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_vector_viewer_base.md), [**NonConstViewer**](classmuda_1_1_dense_vector_viewer_base.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef Eigen::Vector&lt; T, Eigen::Dynamic &gt; | [**VectorType**](#typedef-vectortype)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseVectorViewerBase**](#function-densevectorviewerbase) (auto\_const\_t&lt; T &gt; \* data, int offset, int size, int origin\_size) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC Eigen::VectorBlock&lt; CMapVector &gt; | [**as\_eigen**](#function-as_eigen-12) () const<br> |
|  MUDA\_GENERIC Eigen::VectorBlock&lt; ThisMapVector &gt; | [**as\_eigen**](#function-as_eigen-22) () <br> |
|  MUDA\_GENERIC auto | [**offset**](#function-offset) () const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC | [**VectorBlock&lt; CMapVector &gt;**](#function-vectorblock<-cmapvector->) () const<br> |
|  MUDA\_GENERIC | [**VectorBlock&lt; ThisMapVector &gt;**](#function-vectorblock<-thismapvector->) () <br> |
|  MUDA\_GENERIC const T & | [**operator()**](#function-operator()-12) (int i) const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()-22) (int i) <br> |
|  MUDA\_GENERIC auto | [**origin\_data**](#function-origin_data) () const<br> |
|  MUDA\_GENERIC auto | [**origin\_size**](#function-origin_size) () const<br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-14) (int offset, int size) <br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-24) (int offset) <br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-34) (int offset, int size) const<br> |
|  MUDA\_GENERIC auto | [**segment**](#function-segment-44) (int offset) const<br> |
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
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_size\_matching**](#function-check_size_matching) (int N) <br> |
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
using muda::DenseVectorViewerBase< IsConst, T >::BufferView =  BufferView<T>;
```




<hr>



### typedef CBufferView 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::CBufferView =  CBufferView<T>;
```




<hr>



### typedef CMapVector 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::CMapVector =  MapVectorT<const VectorType>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::ConstViewer =  DenseVectorViewerBase<true, T>;
```




<hr>



### typedef MapVector 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::MapVector =  MapVectorT<VectorType>;
```




<hr>



### typedef MapVectorT 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::MapVectorT =  Eigen::Map<U, Eigen::AlignmentType::Unaligned, Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic> >;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::NonConstViewer =  DenseVectorViewerBase<false, T>;
```




<hr>



### typedef ThisBufferView 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::ThisBufferView =  std::conditional_t<IsConst, CBufferView, BufferView>;
```




<hr>



### typedef ThisMapVector 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::ThisMapVector =  std::conditional_t<IsConst, CMapVector, MapVector>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::ThisViewer =  std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>



### typedef VectorType 

```C++
using muda::DenseVectorViewerBase< IsConst, T >::VectorType =  Eigen::Vector<T, Eigen::Dynamic>;
```




<hr>
## Public Functions Documentation




### function DenseVectorViewerBase 

```C++
inline MUDA_GENERIC muda::DenseVectorViewerBase::DenseVectorViewerBase (
    auto_const_t< T > * data,
    int offset,
    int size,
    int origin_size
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::as_const () const
```




<hr>



### function as\_eigen [1/2]

```C++
inline MUDA_GENERIC Eigen::VectorBlock< CMapVector > muda::DenseVectorViewerBase::as_eigen () const
```




<hr>



### function as\_eigen [2/2]

```C++
inline MUDA_GENERIC Eigen::VectorBlock< ThisMapVector > muda::DenseVectorViewerBase::as_eigen () 
```




<hr>



### function offset 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::offset () const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::DenseVectorViewerBase::operator ConstViewer () const
```




<hr>



### function VectorBlock&lt; CMapVector &gt; 

```C++
inline MUDA_GENERIC muda::DenseVectorViewerBase::VectorBlock< CMapVector > () const
```




<hr>



### function VectorBlock&lt; ThisMapVector &gt; 

```C++
inline MUDA_GENERIC muda::DenseVectorViewerBase::VectorBlock< ThisMapVector > () 
```




<hr>



### function operator() [1/2]

```C++
inline MUDA_GENERIC const T & muda::DenseVectorViewerBase::operator() (
    int i
) const
```




<hr>



### function operator() [2/2]

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::DenseVectorViewerBase::operator() (
    int i
) 
```




<hr>



### function origin\_data 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::origin_data () const
```




<hr>



### function origin\_size 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::origin_size () const
```




<hr>



### function segment [1/4]

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::segment (
    int offset,
    int size
) 
```




<hr>



### function segment [2/4]

```C++
template<int N>
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::segment (
    int offset
) 
```




<hr>



### function segment [3/4]

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::segment (
    int offset,
    int size
) const
```




<hr>



### function segment [4/4]

```C++
template<int N>
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::segment (
    int offset
) const
```




<hr>



### function size 

```C++
inline MUDA_GENERIC auto muda::DenseVectorViewerBase::size () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::DenseVectorViewerBase< IsConst, T >::m_data;
```




<hr>



### variable m\_offset 

```C++
int muda::DenseVectorViewerBase< IsConst, T >::m_offset;
```




<hr>



### variable m\_origin\_size 

```C++
int muda::DenseVectorViewerBase< IsConst, T >::m_origin_size;
```




<hr>



### variable m\_size 

```C++
int muda::DenseVectorViewerBase< IsConst, T >::m_size;
```




<hr>
## Protected Functions Documentation




### function check\_data 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseVectorViewerBase::check_data () const
```




<hr>



### function check\_segment 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseVectorViewerBase::check_segment (
    int offset,
    int size
) const
```




<hr>



### function check\_size\_matching 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseVectorViewerBase::check_size_matching (
    int N
) 
```




<hr>



### function index 

```C++
inline MUDA_INLINE MUDA_GENERIC int muda::DenseVectorViewerBase::index (
    int i
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_vector_viewer.h`

