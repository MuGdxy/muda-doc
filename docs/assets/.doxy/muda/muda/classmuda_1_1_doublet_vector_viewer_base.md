

# Class muda::DoubletVectorViewerBase

**template &lt;bool IsConst, typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)












## Classes

| Type | Name |
| ---: | :--- |
| struct | [**CDoublet**](structmuda_1_1_doublet_vector_viewer_base_1_1_c_doublet.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; true, T, N &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; false, T, N &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef Eigen::Matrix&lt; T, N, 1 &gt; | [**SegmentVector**](#typedef-segmentvector)  <br> |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; IsConst, T, N &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DoubletVectorViewerBase**](#function-doubletvectorviewerbase-12) () = default<br> |
|  MUDA\_GENERIC | [**DoubletVectorViewerBase**](#function-doubletvectorviewerbase-22) (int total\_segment\_count, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, int subvector\_offset, int subvector\_extent, auto\_const\_t&lt; int &gt; \* segment\_indices, auto\_const\_t&lt; SegmentVector &gt; \* segment\_values) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_doublet_vector_viewer_base.md) | [**as\_const**](#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC int | [**doublet\_count**](#function-doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () noexcept const<br> |
|  MUDA\_GENERIC [**CDoublet**](structmuda_1_1_doublet_vector_viewer_base_1_1_c_doublet.md) | [**operator()**](#function-operator()) (int i) const<br> |
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
|  auto\_const\_t&lt; SegmentVector &gt; \* | [**m\_segment\_values**](#variable-m_segment_values)  <br> |
|  int | [**m\_subvector\_extent**](#variable-m_subvector_extent)   = = 0<br> |
|  int | [**m\_subvector\_offset**](#variable-m_subvector_offset)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](#variable-m_total_doublet_count)   = = 0<br> |
|  int | [**m\_total\_segment\_count**](#variable-m_total_segment_count)   = = 0<br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
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
using muda::DoubletVectorViewerBase< IsConst, T, N >::ConstViewer =  DoubletVectorViewerBase<true, T, N>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DoubletVectorViewerBase< IsConst, T, N >::NonConstViewer =  DoubletVectorViewerBase<false, T, N>;
```




<hr>



### typedef SegmentVector 

```C++
using muda::DoubletVectorViewerBase< IsConst, T, N >::SegmentVector =  Eigen::Matrix<T, N, 1>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DoubletVectorViewerBase< IsConst, T, N >::ThisViewer =  DoubletVectorViewerBase<IsConst, T, N>;
```




<hr>
## Public Functions Documentation




### function DoubletVectorViewerBase [1/2]

```C++
MUDA_GENERIC muda::DoubletVectorViewerBase::DoubletVectorViewerBase () = default
```




<hr>



### function DoubletVectorViewerBase [2/2]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewerBase::DoubletVectorViewerBase (
    int total_segment_count,
    int doublet_index_offset,
    int doublet_count,
    int total_doublet_count,
    int subvector_offset,
    int subvector_extent,
    auto_const_t< int > * segment_indices,
    auto_const_t< SegmentVector > * segment_values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstViewer muda::DoubletVectorViewerBase::as_const () noexcept const
```




<hr>



### function doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase::doublet_count () noexcept const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::DoubletVectorViewerBase::operator ConstViewer () noexcept const
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC CDoublet muda::DoubletVectorViewerBase::operator() (
    int i
) const
```




<hr>



### function total\_doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase::total_doublet_count () noexcept const
```




<hr>
## Protected Attributes Documentation




### variable m\_doublet\_count 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, N >::m_doublet_count;
```




<hr>



### variable m\_doublet\_index\_offset 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, N >::m_doublet_index_offset;
```




<hr>



### variable m\_segment\_indices 

```C++
auto_const_t<int>* muda::DoubletVectorViewerBase< IsConst, T, N >::m_segment_indices;
```




<hr>



### variable m\_segment\_values 

```C++
auto_const_t<SegmentVector>* muda::DoubletVectorViewerBase< IsConst, T, N >::m_segment_values;
```




<hr>



### variable m\_subvector\_extent 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, N >::m_subvector_extent;
```




<hr>



### variable m\_subvector\_offset 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, N >::m_subvector_offset;
```




<hr>



### variable m\_total\_doublet\_count 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, N >::m_total_doublet_count;
```




<hr>



### variable m\_total\_segment\_count 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, N >::m_total_segment_count;
```




<hr>
## Protected Functions Documentation




### function check\_in\_subvector 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DoubletVectorViewerBase::check_in_subvector (
    int i
) noexcept const
```




<hr>



### function get\_index 

```C++
inline MUDA_INLINE MUDA_GENERIC int muda::DoubletVectorViewerBase::get_index (
    int i
) noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/doublet_vector_viewer.h`

