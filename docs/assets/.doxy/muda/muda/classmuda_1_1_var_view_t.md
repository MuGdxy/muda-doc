

# Class muda::VarViewT

**template &lt;bool IsConst, typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**VarViewT**](classmuda_1_1_var_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**VarViewT**](classmuda_1_1_var_view_t.md)&lt; true, T &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**CDense**](classmuda_1_1_dense_viewer_t.md)&lt; T &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**Dense**](classmuda_1_1_dense_viewer_t.md)&lt; T &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**VarViewT**](classmuda_1_1_var_view_t.md)&lt; IsConst, T &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef typename std::conditional\_t&lt; IsConst, [**ConstViewer**](classmuda_1_1_dense_viewer_t.md), [**NonConstViewer**](classmuda_1_1_dense_viewer_t.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef size\_t | [**difference\_type**](#typedef-difference_type)  <br> |
| typedef std::random\_access\_iterator\_tag | [**iterator\_category**](#typedef-iterator_category)  <br> |
| typedef T \* | [**pointer**](#typedef-pointer)  <br> |
| typedef T & | [**reference**](#typedef-reference)  <br> |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |


## Public Types inherited from muda::ViewBase

See [muda::ViewBase](classmuda_1_1_view_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_view_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_view_base.md#typedef-non_const_enable_t)  <br> |












## Public Static Attributes inherited from muda::ViewBase

See [muda::ViewBase](classmuda_1_1_view_base.md)

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](classmuda_1_1_view_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_view_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**VarViewT**](#function-varviewt-25) () <br> |
|  MUDA\_GENERIC | [**VarViewT**](#function-varviewt-35) (auto\_const\_t&lt; T &gt; \* data) <br> |
|  MUDA\_GENERIC | [**VarViewT**](#function-varviewt-45) (const [**VarViewT**](classmuda_1_1_var_view_t.md) & other) <br> |
|  MUDA\_GENERIC | [**VarViewT**](#function-varviewt-55) (const [**VarViewT**](classmuda_1_1_var_view_t.md)&lt; OtherIsConst, T &gt; & other) <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_var_view_t.md) | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-12) (const T \* data) const<br> |
|  MUDA\_HOST void | [**copy\_from**](#function-copy_from-22) (const [**ConstView**](classmuda_1_1_var_view_t.md) & val) const<br> |
|  MUDA\_HOST void | [**copy\_to**](#function-copy_to) (T \* data) const<br> |
|  MUDA\_GENERIC [**ConstViewer**](classmuda_1_1_dense_viewer_t.md) | [**cviewer**](#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; \* | [**data**](#function-data) () const<br> |
|  MUDA\_HOST void | [**fill**](#function-fill) (const T & value) const<br> |
|  MUDA\_GENERIC reference | [**operator\***](#function-operator) () <br> |
|  MUDA\_GENERIC auto\_const\_t&lt; T &gt; & | [**operator[]**](#function-operator_1) (int i) const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](#function-viewer) () const<br> |








## Protected Types

| Type | Name |
| ---: | :--- |
| typedef typename Base::template auto\_const\_t&lt; U &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  auto\_const\_t&lt; T &gt; \* | [**m\_data**](#variable-m_data)   = = nullptr<br> |








































## Public Types Documentation




### typedef ConstView 

```C++
using muda::VarViewT< IsConst, T >::ConstView =  VarViewT<true, T>;
```




<hr>



### typedef ConstViewer 

```C++
using muda::VarViewT< IsConst, T >::ConstViewer =  CDense<T>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::VarViewT< IsConst, T >::NonConstViewer =  Dense<T>;
```




<hr>



### typedef ThisView 

```C++
using muda::VarViewT< IsConst, T >::ThisView =  VarViewT<IsConst, T>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::VarViewT< IsConst, T >::ThisViewer =  typename std::conditional_t<IsConst, ConstViewer, NonConstViewer>;
```




<hr>



### typedef difference\_type 

```C++
using muda::VarViewT< IsConst, T >::difference_type =  size_t;
```




<hr>



### typedef iterator\_category 

```C++
using muda::VarViewT< IsConst, T >::iterator_category =  std::random_access_iterator_tag;
```




<hr>



### typedef pointer 

```C++
using muda::VarViewT< IsConst, T >::pointer =  T*;
```




<hr>



### typedef reference 

```C++
using muda::VarViewT< IsConst, T >::reference =  T&;
```




<hr>



### typedef value\_type 

```C++
using muda::VarViewT< IsConst, T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function VarViewT [2/5]

```C++
MUDA_GENERIC muda::VarViewT::VarViewT () 
```




<hr>



### function VarViewT [3/5]

```C++
MUDA_GENERIC muda::VarViewT::VarViewT (
    auto_const_t< T > * data
) 
```




<hr>



### function VarViewT [4/5]

```C++
MUDA_GENERIC muda::VarViewT::VarViewT (
    const VarViewT & other
) 
```




<hr>



### function VarViewT [5/5]

```C++
template<bool OtherIsConst>
MUDA_GENERIC muda::VarViewT::VarViewT (
    const VarViewT < OtherIsConst, T > & other
) 
```




<hr>



### function as\_const 

```C++
MUDA_GENERIC ConstView muda::VarViewT::as_const () const
```




<hr>



### function copy\_from [1/2]

```C++
MUDA_HOST void muda::VarViewT::copy_from (
    const T * data
) const
```




<hr>



### function copy\_from [2/2]

```C++
MUDA_HOST void muda::VarViewT::copy_from (
    const ConstView & val
) const
```




<hr>



### function copy\_to 

```C++
MUDA_HOST void muda::VarViewT::copy_to (
    T * data
) const
```




<hr>



### function cviewer 

```C++
MUDA_GENERIC ConstViewer muda::VarViewT::cviewer () const
```




<hr>



### function data 

```C++
MUDA_GENERIC auto_const_t< T > * muda::VarViewT::data () const
```




<hr>



### function fill 

```C++
MUDA_HOST void muda::VarViewT::fill (
    const T & value
) const
```




<hr>



### function operator\* 

```C++
inline MUDA_GENERIC reference muda::VarViewT::operator* () 
```




<hr>



### function operator[] 

```C++
inline MUDA_GENERIC auto_const_t< T > & muda::VarViewT::operator[] (
    int i
) const
```




<hr>



### function viewer 

```C++
MUDA_GENERIC ThisViewer muda::VarViewT::viewer () const
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::VarViewT< IsConst, T >::auto_const_t =  typename Base::template auto_const_t<U>;
```




<hr>
## Protected Attributes Documentation




### variable m\_data 

```C++
auto_const_t<T>* muda::VarViewT< IsConst, T >::m_data;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/var_view.h`

