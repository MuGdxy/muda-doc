

# Class muda::ViewerBase

**template &lt;bool IsConst\_&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ViewerBase**](classmuda_1_1_viewer_base.md)




























## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsConst**](#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](#variable-isnonconst)   = = !IsConst\_<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**ViewerBase**](#function-viewerbase-13) () <br> |
|   | [**ViewerBase**](#function-viewerbase-23) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|   | [**ViewerBase**](#function-viewerbase-33) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**copy\_label**](#function-copy_label) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) & other) <br> |
|  MUDA\_GENERIC const char \* | [**kernel\_file**](#function-kernel_file) () const<br> |
|  MUDA\_GENERIC int | [**kernel\_line**](#function-kernel_line) () const<br> |
|  MUDA\_GENERIC const char \* | [**kernel\_name**](#function-kernel_name) () const<br> |
|  MUDA\_GENERIC const char \* | [**name**](#function-name-13) () const<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](#function-operator) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](#function-operator_1) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |




## Protected Types

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](#typedef-non_const_enable_t)  <br> |




















## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |




## Public Static Attributes Documentation




### variable IsConst 

```C++
constexpr bool muda::ViewerBase< IsConst_ >::IsConst;
```




<hr>



### variable IsNonConst 

```C++
constexpr bool muda::ViewerBase< IsConst_ >::IsNonConst;
```




<hr>
## Public Functions Documentation




### function ViewerBase [1/3]

```C++
inline MUDA_GENERIC muda::ViewerBase::ViewerBase () 
```




<hr>



### function ViewerBase [2/3]

```C++
muda::ViewerBase::ViewerBase (
    const ViewerBase &
) = default
```




<hr>



### function ViewerBase [3/3]

```C++
muda::ViewerBase::ViewerBase (
    ViewerBase &&
) = default
```




<hr>



### function copy\_label 

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::ViewerBase::copy_label (
    const ViewerBase & other
) 
```




<hr>



### function kernel\_file 

```C++
inline MUDA_GENERIC const char * muda::ViewerBase::kernel_file () const
```




<hr>



### function kernel\_line 

```C++
inline MUDA_GENERIC int muda::ViewerBase::kernel_line () const
```




<hr>



### function kernel\_name 

```C++
inline MUDA_GENERIC const char * muda::ViewerBase::kernel_name () const
```




<hr>



### function name [1/3]

```C++
inline MUDA_GENERIC const char * muda::ViewerBase::name () const
```




<hr>



### function operator= 

```C++
ViewerBase & muda::ViewerBase::operator= (
    const ViewerBase &
) = default
```




<hr>



### function operator= 

```C++
ViewerBase & muda::ViewerBase::operator= (
    ViewerBase &&
) = default
```




<hr>
## Protected Types Documentation




### typedef auto\_const\_t 

```C++
using muda::ViewerBase< IsConst_ >::auto_const_t =  std::conditional_t<IsConst, const T, T>;
```




<hr>



### typedef non\_const\_enable\_t 

```C++
using muda::ViewerBase< IsConst_ >::non_const_enable_t =  std::enable_if_t<IsNonConst, T>;
```




<hr>
## Protected Functions Documentation




### function name [2/3]

```C++
inline MUDA_INLINE MUDA_HOST void muda::ViewerBase::name (
    const char * n
) 
```




<hr>



### function name [3/3]

```C++
inline MUDA_INLINE MUDA_GENERIC void muda::ViewerBase::name (
    details::StringPointer pointer
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/viewer/viewer_base.h`

