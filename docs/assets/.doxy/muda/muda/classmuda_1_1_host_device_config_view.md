

# Class muda::HostDeviceConfigView

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**HostDeviceConfigView**](classmuda_1_1_host_device_config_view.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
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
|  MUDA\_GENERIC | [**HostDeviceConfigView**](#function-hostdeviceconfigview) (const T \* host\_data, const T \* device\_data) <br> |
|  MUDA\_GENERIC const T \* | [**data**](#function-data) () const<br> |
|  MUDA\_GENERIC const T \* | [**device\_data**](#function-device_data) () const<br> |
|  MUDA\_GENERIC const T \* | [**host\_data**](#function-host_data) () const<br> |
|  MUDA\_GENERIC const T & | [**operator\***](#function-operator) () const<br> |
|  MUDA\_GENERIC const T \* | [**operator-&gt;**](#function-operator_1) () const<br> |
























































## Public Types Documentation




### typedef value\_type 

```C++
using muda::HostDeviceConfigView< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function HostDeviceConfigView 

```C++
inline MUDA_GENERIC muda::HostDeviceConfigView::HostDeviceConfigView (
    const T * host_data,
    const T * device_data
) 
```




<hr>



### function data 

```C++
inline MUDA_GENERIC const T * muda::HostDeviceConfigView::data () const
```




<hr>



### function device\_data 

```C++
inline MUDA_GENERIC const T * muda::HostDeviceConfigView::device_data () const
```




<hr>



### function host\_data 

```C++
inline MUDA_GENERIC const T * muda::HostDeviceConfigView::host_data () const
```




<hr>



### function operator\* 

```C++
inline MUDA_GENERIC const T & muda::HostDeviceConfigView::operator* () const
```




<hr>



### function operator-&gt; 

```C++
inline MUDA_GENERIC const T * muda::HostDeviceConfigView::operator-> () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/host_device_config.h`

