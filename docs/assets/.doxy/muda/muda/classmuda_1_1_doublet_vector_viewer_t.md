

# Class muda::DoubletVectorViewerT

**template &lt;bool IsConst, typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DoubletVectorViewerT**](classmuda_1_1_doublet_vector_viewer_t.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)












## Classes

| Type | Name |
| ---: | :--- |
| struct | [**CDoublet**](structmuda_1_1_doublet_vector_viewer_t_1_1_c_doublet.md) <br> |
| class | [**Proxy**](classmuda_1_1_doublet_vector_viewer_t_1_1_proxy.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**DoubletVectorViewerT**](classmuda_1_1_doublet_vector_viewer_t.md)&lt; true, T, N &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewerT**](classmuda_1_1_doublet_vector_viewer_t.md)&lt; false, T, N &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**DoubletVectorViewerT**](classmuda_1_1_doublet_vector_viewer_t.md)&lt; IsConst, T, N &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef std::conditional\_t&lt; N==1, T, Eigen::Matrix&lt; T, N, 1 &gt; &gt; | [**ValueT**](#typedef-valuet)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DoubletVectorViewerT**](#function-doubletvectorviewert-24) () = default<br> |
|  MUDA\_GENERIC | [**DoubletVectorViewerT**](#function-doubletvectorviewert-34) (int total\_segment\_count, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, int subvector\_offset, int subvector\_extent, auto\_const\_t&lt; int &gt; \* segment\_indices, auto\_const\_t&lt; ValueT &gt; \* segment\_values) <br> |
|  MUDA\_GENERIC | [**DoubletVectorViewerT**](#function-doubletvectorviewert-44) (const [**DoubletVectorViewerT**](classmuda_1_1_doublet_vector_viewer_t.md)&lt; OtherIsConst, T, N &gt; & other) noexcept<br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_doublet_vector_viewer_t.md) | [**as\_const**](#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC int | [**doublet\_count**](#function-doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC auto | [**operator()**](#function-operator()) (int i) const<br> |
|  MUDA\_GENERIC int | [**total\_doublet\_count**](#function-total_doublet_count) () noexcept const<br> |


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
|  int | [**m\_doublet\_count**](#variable-m_doublet_count)   = = 0<br> |
|  int | [**m\_doublet\_index\_offset**](#variable-m_doublet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_segment\_indices**](#variable-m_segment_indices)  <br> |
|  auto\_const\_t&lt; ValueT &gt; \* | [**m\_segment\_values**](#variable-m_segment_values)  <br> |
|  int | [**m\_subvector\_extent**](#variable-m_subvector_extent)   = = 0<br> |
|  int | [**m\_subvector\_offset**](#variable-m_subvector_offset)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](#variable-m_total_doublet_count)   = = 0<br> |
|  int | [**m\_total\_segment\_count**](#variable-m_total_segment_count)   = = 0<br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC [**CDoublet**](structmuda_1_1_doublet_vector_viewer_t_1_1_c_doublet.md) | [**at**](#function-at) (int i) const<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_in\_subvector**](#function-check_in_subvector) (int i) noexcept const<br> |
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
using muda::DoubletVectorViewerT< IsConst, T, N >::ConstViewer =  DoubletVectorViewerT<true, T, N>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DoubletVectorViewerT< IsConst, T, N >::NonConstViewer =  DoubletVectorViewerT<false, T, N>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DoubletVectorViewerT< IsConst, T, N >::ThisViewer =  DoubletVectorViewerT<IsConst, T, N>;
```




<hr>



### typedef ValueT 

```C++
using muda::DoubletVectorViewerT< IsConst, T, N >::ValueT =  std::conditional_t<N == 1, T, Eigen::Matrix<T, N, 1>>;
```




<hr>
## Public Functions Documentation




### function DoubletVectorViewerT [2/4]

```C++
MUDA_GENERIC muda::DoubletVectorViewerT::DoubletVectorViewerT () = default
```




<hr>



### function DoubletVectorViewerT [3/4]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewerT::DoubletVectorViewerT (
    int total_segment_count,
    int doublet_index_offset,
    int doublet_count,
    int total_doublet_count,
    int subvector_offset,
    int subvector_extent,
    auto_const_t< int > * segment_indices,
    auto_const_t< ValueT > * segment_values
) 
```




<hr>



### function DoubletVectorViewerT [4/4]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::DoubletVectorViewerT::DoubletVectorViewerT (
    const DoubletVectorViewerT < OtherIsConst, T, N > & other
) noexcept
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstViewer muda::DoubletVectorViewerT::as_const () noexcept const
```




<hr>



### function doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerT::doublet_count () noexcept const
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC auto muda::DoubletVectorViewerT::operator() (
    int i
) const
```




<hr>



### function total\_doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerT::total_doublet_count () noexcept const
```




<hr>
## Protected Attributes Documentation




### variable m\_doublet\_count 

```C++
int muda::DoubletVectorViewerT< IsConst, T, N >::m_doublet_count;
```




<hr>



### variable m\_doublet\_index\_offset 

```C++
int muda::DoubletVectorViewerT< IsConst, T, N >::m_doublet_index_offset;
```




<hr>



### variable m\_segment\_indices 

```C++
auto_const_t<int>* muda::DoubletVectorViewerT< IsConst, T, N >::m_segment_indices;
```




<hr>



### variable m\_segment\_values 

```C++
auto_const_t<ValueT>* muda::DoubletVectorViewerT< IsConst, T, N >::m_segment_values;
```




<hr>



### variable m\_subvector\_extent 

```C++
int muda::DoubletVectorViewerT< IsConst, T, N >::m_subvector_extent;
```




<hr>



### variable m\_subvector\_offset 

```C++
int muda::DoubletVectorViewerT< IsConst, T, N >::m_subvector_offset;
```




<hr>



### variable m\_total\_doublet\_count 

```C++
int muda::DoubletVectorViewerT< IsConst, T, N >::m_total_doublet_count;
```




<hr>



### variable m\_total\_segment\_count 

```C++
int muda::DoubletVectorViewerT< IsConst, T, N >::m_total_segment_count;
```




<hr>
## Protected Functions Documentation




### function at 

```C++
inline MUDA_INLINE MUDA_GENERIC CDoublet muda::DoubletVectorViewerT::at (
    int i
) const
```




<hr>



### function check\_in\_subvector 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DoubletVectorViewerT::check_in_subvector (
    int i
) noexcept const
```




<hr>



### function get\_index 

```C++
inline MUDA_INLINE MUDA_GENERIC int muda::DoubletVectorViewerT::get_index (
    int i
) noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/doublet_vector_viewer.h`

