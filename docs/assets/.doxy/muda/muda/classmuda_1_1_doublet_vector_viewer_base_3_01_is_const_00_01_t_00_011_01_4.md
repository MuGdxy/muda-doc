

# Class muda::DoubletVectorViewerBase&lt; IsConst, T, 1 &gt;

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DoubletVectorViewerBase&lt; IsConst, T, 1 &gt;**](classmuda_1_1_doublet_vector_viewer_base_3_01_is_const_00_01_t_00_011_01_4.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)












## Classes

| Type | Name |
| ---: | :--- |
| struct | [**CDoublet**](structmuda_1_1_doublet_vector_viewer_base_3_01_is_const_00_01_t_00_011_01_4_1_1_c_doublet.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; true, T, 1 &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; IsConst, T, 1 &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**DoubletVectorViewerBase**](classmuda_1_1_doublet_vector_viewer_base.md)&lt; false, T, 1 &gt; | [**Viewer**](#typedef-viewer)  <br> |














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
|  MUDA\_GENERIC | [**DoubletVectorViewerBase**](#function-doubletvectorviewerbase-22) (int total\_count, int doublet\_index\_offset, int doublet\_count, int total\_doublet\_count, int subvector\_offset, int subvector\_extent, auto\_const\_t&lt; int &gt; \* indices, auto\_const\_t&lt; T &gt; \* values) <br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_doublet_vector_viewer_base.md) | [**as\_const**](#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC int | [**doublet\_count**](#function-doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC int | [**extent**](#function-extent) () noexcept const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () noexcept const<br> |
|  MUDA\_GENERIC CDoublet | [**operator()**](#function-operator()) (int i) const<br> |
|  MUDA\_GENERIC int | [**subvector\_offset**](#function-subvector_offset) () noexcept const<br> |
|  MUDA\_GENERIC int | [**total\_doublet\_count**](#function-total_doublet_count) () noexcept const<br> |
|  MUDA\_GENERIC int | [**total\_extent**](#function-total_extent) () noexcept const<br> |


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






## Protected Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |


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
|  auto\_const\_t&lt; int &gt; \* | [**m\_indices**](#variable-m_indices)  <br> |
|  int | [**m\_subvector\_extent**](#variable-m_subvector_extent)   = = 0<br> |
|  int | [**m\_subvector\_offset**](#variable-m_subvector_offset)   = = 0<br> |
|  int | [**m\_total\_count**](#variable-m_total_count)   = = 0<br> |
|  int | [**m\_total\_doublet\_count**](#variable-m_total_doublet_count)   = = 0<br> |
|  auto\_const\_t&lt; T &gt; \* | [**m\_values**](#variable-m_values)  <br> |
































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
using muda::DoubletVectorViewerBase< IsConst, T, 1 >::ConstViewer =  DoubletVectorViewerBase<true, T, 1>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DoubletVectorViewerBase< IsConst, T, 1 >::ThisViewer =  DoubletVectorViewerBase<IsConst, T, 1>;
```




<hr>



### typedef Viewer 

```C++
using muda::DoubletVectorViewerBase< IsConst, T, 1 >::Viewer =  DoubletVectorViewerBase<false, T, 1>;
```




<hr>
## Public Functions Documentation




### function DoubletVectorViewerBase [1/2]

```C++
MUDA_GENERIC muda::DoubletVectorViewerBase< IsConst, T, 1 >::DoubletVectorViewerBase () = default
```




<hr>



### function DoubletVectorViewerBase [2/2]

```C++
inline MUDA_GENERIC muda::DoubletVectorViewerBase< IsConst, T, 1 >::DoubletVectorViewerBase (
    int total_count,
    int doublet_index_offset,
    int doublet_count,
    int total_doublet_count,
    int subvector_offset,
    int subvector_extent,
    auto_const_t< int > * indices,
    auto_const_t< T > * values
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC ConstViewer muda::DoubletVectorViewerBase< IsConst, T, 1 >::as_const () noexcept const
```




<hr>



### function doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase< IsConst, T, 1 >::doublet_count () noexcept const
```




<hr>



### function extent 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase< IsConst, T, 1 >::extent () noexcept const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::DoubletVectorViewerBase< IsConst, T, 1 >::operator ConstViewer () noexcept const
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC CDoublet muda::DoubletVectorViewerBase< IsConst, T, 1 >::operator() (
    int i
) const
```




<hr>



### function subvector\_offset 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase< IsConst, T, 1 >::subvector_offset () noexcept const
```




<hr>



### function total\_doublet\_count 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase< IsConst, T, 1 >::total_doublet_count () noexcept const
```




<hr>



### function total\_extent 

```C++
inline MUDA_GENERIC int muda::DoubletVectorViewerBase< IsConst, T, 1 >::total_extent () noexcept const
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::DoubletVectorViewerBase< IsConst, T, 1 >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_doublet\_count 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_doublet_count;
```




<hr>



### variable m\_doublet\_index\_offset 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_doublet_index_offset;
```




<hr>



### variable m\_indices 

```C++
auto_const_t<int>* muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_indices;
```




<hr>



### variable m\_subvector\_extent 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_subvector_extent;
```




<hr>



### variable m\_subvector\_offset 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_subvector_offset;
```




<hr>



### variable m\_total\_count 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_total_count;
```




<hr>



### variable m\_total\_doublet\_count 

```C++
int muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_total_doublet_count;
```




<hr>



### variable m\_values 

```C++
auto_const_t<T>* muda::DoubletVectorViewerBase< IsConst, T, 1 >::m_values;
```




<hr>
## Protected Functions Documentation




### function check\_in\_subvector 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DoubletVectorViewerBase< IsConst, T, 1 >::check_in_subvector (
    int i
) noexcept const
```




<hr>



### function get\_index 

```C++
inline MUDA_INLINE MUDA_GENERIC int muda::DoubletVectorViewerBase< IsConst, T, 1 >::get_index (
    int i
) noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/doublet_vector_viewer.h`

