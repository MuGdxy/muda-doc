

# Class muda::ViewBase

**template &lt;bool IsConst\_&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ViewBase**](classmuda_1_1_view_base.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](#typedef-non_const_enable_t)  <br> |






## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](#variable-isnonconst)   = = !IsConst\_<br> |










































## Public Types Documentation




### typedef auto\_const\_t 

```C++
using muda::ViewBase< IsConst_ >::auto_const_t =  std::conditional_t<IsConst, const T, T>;
```




<hr>



### typedef non\_const\_enable\_t 

```C++
using muda::ViewBase< IsConst_ >::non_const_enable_t =  std::enable_if_t<IsNonConst, T>;
```




<hr>
## Public Static Attributes Documentation




### variable IsConst 

```C++
bool muda::ViewBase< IsConst_ >::IsConst;
```




<hr>



### variable IsNonConst 

```C++
bool muda::ViewBase< IsConst_ >::IsNonConst;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/view/view_base.h`

