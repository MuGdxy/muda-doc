

# Class muda::Dense1DT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Dense1DT**](classmuda_1_1_dense1_d_t.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**Dense1DT**](classmuda_1_1_dense1_d_t.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**Dense1DT**](classmuda_1_1_dense1_d_t.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**Dense1DT**](classmuda_1_1_dense1_d_t.md)&lt; IsConst, T &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Dense1DT**](#function-dense1dt-14) () <br> |
|  MUDA\_GENERIC | [**Dense1DT**](#function-dense1dt-24) (auto\_const\_t&lt; T &gt; \* p, int dim) <br> |
|  MUDA\_GENERIC | [**Dense1DT**](#function-dense1dt-34) (const [**Dense1DT**](classmuda_1_1_dense1_d_t.md) & other) = default<br> |
|  MUDA\_GENERIC | [**Dense1DT**](#function-dense1dt-44) (const [**Dense1DT**](classmuda_1_1_dense1_d_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data) () const<br> |
|  MUDA\_GENERIC int | [**dim**](#function-dim) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()) (int x) const<br> |
|  MUDA\_GENERIC [**ThisViewer**](classmuda_1_1_dense1_d_t.md) | [**subview**](#function-subview-12) (int offset) const<br> |
|  MUDA\_GENERIC [**ThisViewer**](classmuda_1_1_dense1_d_t.md) | [**subview**](#function-subview-22) (int offset, int size) const<br> |
|  MUDA\_GENERIC int | [**total\_size**](#function-total_size) () const<br> |


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
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |
|  int | [**m\_dim**](#variable-m_dim)   = = 0<br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check**](#function-check) () const<br> |
|  MUDA\_GENERIC int | [**map**](#function-map) (int x) const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef ConstViewer 

```C++
using muda::Dense1DT< IsConst, T >::ConstViewer =  Dense1DT<true, T>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::Dense1DT< IsConst, T >::NonConstViewer =  Dense1DT<false, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::Dense1DT< IsConst, T >::ThisViewer =  Dense1DT<IsConst, T>;
```




<hr>



### typedef value\_type 

```C++
using muda::Dense1DT< IsConst, T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function Dense1DT [1/4]

```C++
MUDA_GENERIC muda::Dense1DT::Dense1DT () 
```




<hr>



### function Dense1DT [2/4]

```C++
inline MUDA_GENERIC muda::Dense1DT::Dense1DT (
    auto_const_t< T > * p,
    int dim
) 
```




<hr>



### function Dense1DT [3/4]

```C++
MUDA_GENERIC muda::Dense1DT::Dense1DT (
    const Dense1DT & other
) = default
```




<hr>



### function Dense1DT [4/4]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::Dense1DT::Dense1DT (
    const Dense1DT < OtherIsConst, T > & other
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::Dense1DT::as_const () const
```




<hr>



### function data 

```C++
inline MUDA_GENERIC auto_const_t< T > * muda::Dense1DT::data () const
```




<hr>



### function dim 

```C++
inline MUDA_GENERIC int muda::Dense1DT::dim () const
```




<hr>



### function operator() 

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::Dense1DT::operator() (
    int x
) const
```




<hr>



### function subview [1/2]

```C++
inline MUDA_GENERIC ThisViewer muda::Dense1DT::subview (
    int offset
) const
```




<hr>



### function subview [2/2]

```C++
inline MUDA_GENERIC ThisViewer muda::Dense1DT::subview (
    int offset,
    int size
) const
```




<hr>



### function total\_size 

```C++
inline MUDA_GENERIC int muda::Dense1DT::total_size () const
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::Dense1DT< IsConst, T >::m_data;
```




<hr>



### variable m\_dim 

```C++
int muda::Dense1DT< IsConst, T >::m_dim;
```




<hr>
## Protected Functions Documentation




### function check 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::Dense1DT::check () const
```




<hr>



### function map 

```C++
inline MUDA_GENERIC int muda::Dense1DT::map (
    int x
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/viewer/dense/dense_1d.h`

