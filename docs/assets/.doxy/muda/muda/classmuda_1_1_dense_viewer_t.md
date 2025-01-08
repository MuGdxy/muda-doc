

# Class muda::DenseViewerT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseViewerT**](classmuda_1_1_dense_viewer_t.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**DenseViewerT**](classmuda_1_1_dense_viewer_t.md)&lt; true, T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**DenseViewerT**](classmuda_1_1_dense_viewer_t.md)&lt; false, T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**DenseViewerT**](classmuda_1_1_dense_viewer_t.md)&lt; IsConst, T &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
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
|  MUDA\_GENERIC | [**DenseViewerT**](#function-denseviewert-25) () <br> |
|  MUDA\_GENERIC | [**DenseViewerT**](#function-denseviewert-35) (auto\_const\_t&lt; T &gt; \* p) <br> |
|  MUDA\_GENERIC | [**DenseViewerT**](#function-denseviewert-45) (const [**DenseViewerT**](classmuda_1_1_dense_viewer_t.md) &) <br> |
|  MUDA\_GENERIC | [**DenseViewerT**](#function-denseviewert-55) (const [**DenseViewerT**](classmuda_1_1_dense_viewer_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data) () const<br> |
|  MUDA\_GENERIC | [**operator auto\_const\_t&lt; T &gt; &**](#function-operator-auto_const_t<-t->-&) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator\***](#function-operator) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**operator-&gt;**](#function-operator_1) () const<br> |
|  MUDA\_GENERIC [**ThisViewer**](classmuda_1_1_dense_viewer_t.md) & | [**operator=**](#function-operator_2) (const T & v) <br> |


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
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC void | [**check**](#function-check) () const<br> |


## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef ConstViewer 

```C++
using muda::DenseViewerT< IsConst, T >::ConstViewer =  DenseViewerT<true, T>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::DenseViewerT< IsConst, T >::NonConstViewer =  DenseViewerT<false, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseViewerT< IsConst, T >::ThisViewer =  DenseViewerT<IsConst, T>;
```




<hr>



### typedef value\_type 

```C++
using muda::DenseViewerT< IsConst, T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function DenseViewerT [2/5]

```C++
MUDA_GENERIC muda::DenseViewerT::DenseViewerT () 
```




<hr>



### function DenseViewerT [3/5]

```C++
inline explicit MUDA_GENERIC muda::DenseViewerT::DenseViewerT (
    auto_const_t< T > * p
) 
```




<hr>



### function DenseViewerT [4/5]

```C++
MUDA_GENERIC muda::DenseViewerT::DenseViewerT (
    const DenseViewerT &
) 
```




<hr>



### function DenseViewerT [5/5]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::DenseViewerT::DenseViewerT (
    const DenseViewerT < OtherIsConst, T > & other
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::DenseViewerT::as_const () const
```




<hr>



### function data 

```C++
inline MUDA_GENERIC auto_const_t< T > * muda::DenseViewerT::data () const
```




<hr>



### function operator auto\_const\_t&lt; T &gt; & 

```C++
inline MUDA_GENERIC muda::DenseViewerT::operator auto_const_t< T > & () const
```




<hr>



### function operator\* 

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::DenseViewerT::operator* () const
```




<hr>



### function operator-&gt; 

```C++
inline MUDA_GENERIC auto_const_t< T > * muda::DenseViewerT::operator-> () const
```




<hr>



### function operator= 

```C++
inline MUDA_GENERIC ThisViewer & muda::DenseViewerT::operator= (
    const T & v
) 
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::DenseViewerT< IsConst, T >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::DenseViewerT< IsConst, T >::m_data;
```




<hr>
## Protected Functions Documentation




### function check 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::DenseViewerT::check () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/viewer/dense/dense_0d.h`

