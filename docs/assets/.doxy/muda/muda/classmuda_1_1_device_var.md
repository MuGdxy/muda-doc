

# Class muda::DeviceVar

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceVar**](classmuda_1_1_device_var.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceVar**](#function-devicevar-14) () <br> |
|   | [**DeviceVar**](#function-devicevar-24) (const T & value) <br> |
|   | [**DeviceVar**](#function-devicevar-34) (const [**DeviceVar**](classmuda_1_1_device_var.md) & other) <br> |
|   | [**DeviceVar**](#function-devicevar-44) ([**DeviceVar**](classmuda_1_1_device_var.md) && other) <br> |
|  void | [**copy\_from**](#function-copy_from) ([**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; other) <br> |
|  [**CDense**](classmuda_1_1_dense_viewer_t.md)&lt; T &gt; | [**cviewer**](#function-cviewer) () const<br> |
|  T \* | [**data**](#function-data-12) () <br> |
|  const T \* | [**data**](#function-data-22) () const<br> |
|   | [**operator CVarView&lt; T &gt;**](#function-operator-cvarview<-t->) () const<br> |
|   | [**operator T**](#function-operator-t) () const<br> |
|   | [**operator VarView&lt; T &gt;**](#function-operator-varview<-t->) () <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md) & | [**operator=**](#function-operator) (const [**DeviceVar**](classmuda_1_1_device_var.md)&lt; T &gt; & other) <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md) & | [**operator=**](#function-operator_1) ([**DeviceVar**](classmuda_1_1_device_var.md)&lt; T &gt; && other) <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md) & | [**operator=**](#function-operator_2) ([**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; other) <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md) & | [**operator=**](#function-operator_3) (const T & val) <br> |
|  [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; | [**view**](#function-view-12) () <br> |
|  [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; | [**view**](#function-view-22) () const<br> |
|  [**Dense**](classmuda_1_1_dense_viewer_t.md)&lt; T &gt; | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceVar**](#function-devicevar) () <br> |




























## Public Types Documentation




### typedef value\_type 

```C++
using muda::DeviceVar< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function DeviceVar [1/4]

```C++
muda::DeviceVar::DeviceVar () 
```




<hr>



### function DeviceVar [2/4]

```C++
muda::DeviceVar::DeviceVar (
    const T & value
) 
```




<hr>



### function DeviceVar [3/4]

```C++
muda::DeviceVar::DeviceVar (
    const DeviceVar & other
) 
```




<hr>



### function DeviceVar [4/4]

```C++
muda::DeviceVar::DeviceVar (
    DeviceVar && other
) 
```




<hr>



### function copy\_from 

```C++
void muda::DeviceVar::copy_from (
    CVarView < T > other
) 
```




<hr>



### function cviewer 

```C++
CDense < T > muda::DeviceVar::cviewer () const
```




<hr>



### function data [1/2]

```C++
inline T * muda::DeviceVar::data () 
```




<hr>



### function data [2/2]

```C++
inline const T * muda::DeviceVar::data () const
```




<hr>



### function operator CVarView&lt; T &gt; 

```C++
inline muda::DeviceVar::operator CVarView< T > () const
```




<hr>



### function operator T 

```C++
muda::DeviceVar::operator T () const
```




<hr>



### function operator VarView&lt; T &gt; 

```C++
inline muda::DeviceVar::operator VarView< T > () 
```




<hr>



### function operator= 

```C++
DeviceVar & muda::DeviceVar::operator= (
    const DeviceVar < T > & other
) 
```




<hr>



### function operator= 

```C++
DeviceVar & muda::DeviceVar::operator= (
    DeviceVar < T > && other
) 
```




<hr>



### function operator= 

```C++
DeviceVar & muda::DeviceVar::operator= (
    CVarView < T > other
) 
```




<hr>



### function operator= 

```C++
DeviceVar & muda::DeviceVar::operator= (
    const T & val
) 
```




<hr>



### function view [1/2]

```C++
inline VarView < T > muda::DeviceVar::view () 
```




<hr>



### function view [2/2]

```C++
inline CVarView < T > muda::DeviceVar::view () const
```




<hr>



### function viewer 

```C++
Dense < T > muda::DeviceVar::viewer () 
```




<hr>



### function ~DeviceVar 

```C++
muda::DeviceVar::~DeviceVar () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/device_var.h`

