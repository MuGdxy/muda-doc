

# Class muda::DoubletVectorViewer&lt; T, 1 &gt;

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DoubletVectorViewer&lt; T, 1 &gt;**](classmuda_1_1_doublet_vector_viewer_3_01_t_00_011_01_4.md)








Inherits the following classes: [muda::DoubletVectorViewerBase](classmuda_1_1_doublet_vector_viewer_base.md)












## Classes

| Type | Name |
| ---: | :--- |
| class | [**Proxy**](classmuda_1_1_doublet_vector_viewer_3_01_t_00_011_01_4_1_1_proxy.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::CDoublet | [**CDoublet**](#typedef-cdoublet)  <br> |
| typedef [**CDoubletVectorViewer**](classmuda_1_1_c_doublet_vector_viewer.md)&lt; T, 1 &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewer**](classmuda_1_1_doublet_vector_viewer.md)&lt; T, 1 &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |


## Public Types inherited from muda::DoubletVectorViewerBase

See [muda::DoubletVectorViewerBase](classmuda_1_1_doublet_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; true, T, N &gt; | [**ConstViewer**](classmuda_1_1_doublet_vector_viewer_base.md#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; false, T, N &gt; | [**NonConstViewer**](classmuda_1_1_doublet_vector_viewer_base.md#typedef-nonconstviewer)  <br> |
| typedef Eigen::Matrix&lt; T, N, 1 &gt; | [**SegmentVector**](classmuda_1_1_doublet_vector_viewer_base.md#typedef-segmentvector)  <br> |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; IsConst, T, N &gt; | [**ThisViewer**](classmuda_1_1_doublet_vector_viewer_base.md#typedef-thisviewer)  <br> |




















## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DoubletVectorViewer**](#function-doubletvectorviewer) (const [**Base**](classmuda_1_1_doublet_vector_viewer_base.md) & base) <br> |
|  MUDA\_GENERIC Proxy | [**operator()**](#function-operator()) (int i) <br> |


## Public Functions inherited from muda::DoubletVectorViewerBase

See [muda::DoubletVectorViewerBase](classmuda_1_1_doublet_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md#function-doubletvectorviewerbase-12) () = default<br> |
|  MUDA\_GENERIC | [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md#function-doubletvectorviewerbase-22) (int total\_segment\_count, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, int subvector\_offset, int subvector\_extent, auto\_const\_t&lt; int &gt; \* segment\_indices, auto\_const\_t&lt; SegmentVector &gt; \* segment\_values) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_doublet_vector_viewer_base.md) | [**as\_const**](classmuda_1_1_doublet_vector_viewer_base.md#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC int | [**doublet\_count**](classmuda_1_1_doublet_vector_viewer_base.md#function-doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](classmuda_1_1_doublet_vector_viewer_base.md#function-operator-constviewer) () noexcept const<br> |
|  MUDA\_GENERIC [**CDoublet**](structmuda_1_1_doublet_vector_viewer_base_1_1_c_doublet.md) | [**operator()**](classmuda_1_1_doublet_vector_viewer_base.md#function-operator()) (int i) const<br> |
|  MUDA\_GENERIC int | [**total\_doublet\_count**](classmuda_1_1_doublet_vector_viewer_base.md#function-total_doublet_count) () noexcept const<br> |


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










## Protected Attributes inherited from muda::DoubletVectorViewerBase

See [muda::DoubletVectorViewerBase](classmuda_1_1_doublet_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  int | [**m\_doublet\_count**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_doublet_count)   = = 0<br> |
|  int | [**m\_doublet\_index\_offset**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_doublet_index_offset)   = = 0<br> |
|  auto\_const\_t&lt; int &gt; \* | [**m\_segment\_indices**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_segment_indices)  <br> |
|  auto\_const\_t&lt; SegmentVector &gt; \* | [**m\_segment\_values**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_segment_values)  <br> |
|  int | [**m\_subvector\_extent**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_subvector_extent)   = = 0<br> |
|  int | [**m\_subvector\_offset**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_subvector_offset)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_total_doublet_count)   = = 0<br> |
|  int | [**m\_total\_segment\_count**](classmuda_1_1_doublet_vector_viewer_base.md#variable-m_total_segment_count)   = = 0<br> |
















































## Protected Functions inherited from muda::DoubletVectorViewerBase

See [muda::DoubletVectorViewerBase](classmuda_1_1_doublet_vector_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_in\_subvector**](classmuda_1_1_doublet_vector_viewer_base.md#function-check_in_subvector) (int i) noexcept const<br> |
|  MUDA\_INLINE MUDA\_GENERIC int | [**get\_index**](classmuda_1_1_doublet_vector_viewer_base.md#function-get_index) (int i) noexcept const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |








## Public Types Documentation




### typedef CDoublet 

```C++
using muda::DoubletVectorViewer< T, 1 >::CDoublet =  typename Base::CDoublet;
```




<hr>



### typedef ConstViewer 

```C++
using muda::DoubletVectorViewer< T, 1 >::ConstViewer =  CDoubletVectorViewer<T, 1>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DoubletVectorViewer< T, 1 >::ThisViewer =  DoubletVectorViewer<T, 1>;
```




<hr>
## Public Functions Documentation




### function DoubletVectorViewer 

```C++
inline MUDA_GENERIC muda::DoubletVectorViewer< T, 1 >::DoubletVectorViewer (
    const Base & base
) 
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC Proxy muda::DoubletVectorViewer< T, 1 >::operator() (
    int i
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/doublet_vector_viewer.h`

