

# Class muda::Dense2DBase

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Dense2DBase**](classmuda_1_1_dense2_d_base.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**Dense2DBase**](classmuda_1_1_dense2_d_base.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**Dense2DBase**](classmuda_1_1_dense2_d_base.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**Dense2DBase**](classmuda_1_1_dense2_d_base.md)&lt; IsConst, T &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Dense2DBase**](#function-dense2dbase-12) () <br> |
|  MUDA\_GENERIC | [**Dense2DBase**](#function-dense2dbase-22) (auto\_const\_t&lt; T &gt; \* p, const int2 & offset, const int2 & dim, int pitch\_bytes) <br> |
|  MUDA\_GENERIC auto | [**area**](#function-area) () const<br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data-12) () <br> |
|  MUDA\_GENERIC const T \* | [**data**](#function-data-22) () const<br> |
|  MUDA\_GENERIC auto | [**dim**](#function-dim) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**flatten**](#function-flatten-12) (int i) <br> |
|  MUDA\_GENERIC const T & | [**flatten**](#function-flatten-22) (int i) const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()-14) (int x, int y) <br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator()**](#function-operator()-24) (const int2 & xy) <br> |
|  MUDA\_GENERIC const T & | [**operator()**](#function-operator()-34) (const int2 & xy) const<br> |
|  MUDA\_GENERIC const T & | [**operator()**](#function-operator()-44) (int x, int y) const<br> |
|  MUDA\_GENERIC auto | [**pitch\_bytes**](#function-pitch_bytes) () const<br> |
|  MUDA\_GENERIC auto | [**total\_size**](#function-total_size) () const<br> |


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
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)  <br> |
|  int2 | [**m\_dim**](#variable-m_dim)  <br> |
|  int2 | [**m\_offset**](#variable-m_offset)  <br> |
|  int | [**m\_pitch\_bytes**](#variable-m_pitch_bytes)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check**](#function-check) () const<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check\_range**](#function-check_range) (int x, int y) const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef ConstViewer 

```C++
using muda::Dense2DBase< IsConst, T >::ConstViewer =  Dense2DBase<true, T>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::Dense2DBase< IsConst, T >::NonConstViewer =  Dense2DBase<false, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::Dense2DBase< IsConst, T >::ThisViewer =  Dense2DBase<IsConst, T>;
```




<hr>



### typedef value\_type 

```C++
using muda::Dense2DBase< IsConst, T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function Dense2DBase [1/2]

```C++
inline MUDA_GENERIC muda::Dense2DBase::Dense2DBase () 
```




<hr>



### function Dense2DBase [2/2]

```C++
inline MUDA_GENERIC muda::Dense2DBase::Dense2DBase (
    auto_const_t< T > * p,
    const int2 & offset,
    const int2 & dim,
    int pitch_bytes
) 
```




<hr>



### function area 

```C++
inline MUDA_GENERIC auto muda::Dense2DBase::area () const
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::Dense2DBase::as_const () const
```




<hr>



### function data [1/2]

```C++
inline MUDA_GENERIC auto_const_t< T > * muda::Dense2DBase::data () 
```




<hr>



### function data [2/2]

```C++
inline MUDA_GENERIC const T * muda::Dense2DBase::data () const
```




<hr>



### function dim 

```C++
inline MUDA_GENERIC auto muda::Dense2DBase::dim () const
```




<hr>



### function flatten [1/2]

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::Dense2DBase::flatten (
    int i
) 
```




<hr>



### function flatten [2/2]

```C++
inline MUDA_GENERIC const T & muda::Dense2DBase::flatten (
    int i
) const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::Dense2DBase::operator ConstViewer () const
```




<hr>



### function operator() [1/4]

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::Dense2DBase::operator() (
    int x,
    int y
) 
```




<hr>



### function operator() [2/4]

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::Dense2DBase::operator() (
    const int2 & xy
) 
```




<hr>



### function operator() [3/4]

```C++
inline MUDA_GENERIC const T & muda::Dense2DBase::operator() (
    const int2 & xy
) const
```




<hr>



### function operator() [4/4]

```C++
inline MUDA_GENERIC const T & muda::Dense2DBase::operator() (
    int x,
    int y
) const
```




<hr>



### function pitch\_bytes 

```C++
inline MUDA_GENERIC auto muda::Dense2DBase::pitch_bytes () const
```




<hr>



### function total\_size 

```C++
inline MUDA_GENERIC auto muda::Dense2DBase::total_size () const
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::Dense2DBase< IsConst, T >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::Dense2DBase< IsConst, T >::m_data;
```




<hr>



### variable m\_dim 

```C++
int2 muda::Dense2DBase< IsConst, T >::m_dim;
```




<hr>



### variable m\_offset 

```C++
int2 muda::Dense2DBase< IsConst, T >::m_offset;
```




<hr>



### variable m\_pitch\_bytes 

```C++
int muda::Dense2DBase< IsConst, T >::m_pitch_bytes;
```




<hr>
## Protected Functions Documentation




### function check 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::Dense2DBase::check () const
```




<hr>



### function check\_range 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::Dense2DBase::check_range (
    int x,
    int y
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/viewer/dense/dense_2d.h`

