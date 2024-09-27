

# Class muda::HostDeviceConfig

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**HostDeviceConfig**](classmuda_1_1_host_device_config.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**HostDeviceConfig**](#function-hostdeviceconfig-14) () = default<br> |
|   | [**HostDeviceConfig**](#function-hostdeviceconfig-24) (const T & value) <br> |
|   | [**HostDeviceConfig**](#function-hostdeviceconfig-34) (const [**HostDeviceConfig**](classmuda_1_1_host_device_config.md) &) = default<br> |
|   | [**HostDeviceConfig**](#function-hostdeviceconfig-44) ([**HostDeviceConfig**](classmuda_1_1_host_device_config.md) &&) <br> |
|  auto | [**buffer\_view**](#function-buffer_view-12) () <br> |
|  auto | [**buffer\_view**](#function-buffer_view-22) () const<br> |
|  const T \* | [**device\_data**](#function-device_data) () const<br> |
|  const T \* | [**host\_data**](#function-host_data-12) () const<br> |
|  T \* | [**host\_data**](#function-host_data-22) () <br> |
|  [**HostDeviceConfig**](classmuda_1_1_host_device_config.md) & | [**operator=**](#function-operator) (const [**HostDeviceConfig**](classmuda_1_1_host_device_config.md)&lt; T &gt; &) = default<br> |
|  [**HostDeviceConfig**](classmuda_1_1_host_device_config.md) & | [**operator=**](#function-operator_1) ([**HostDeviceConfig**](classmuda_1_1_host_device_config.md)&lt; T &gt; &&) = default<br> |
|  [**HostDeviceConfig**](classmuda_1_1_host_device_config.md) & | [**operator=**](#function-operator_2) (const T & val) <br> |
|  auto | [**view**](#function-view) () const<br> |




























## Public Types Documentation




### typedef value\_type 

```C++
using muda::HostDeviceConfig< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function HostDeviceConfig [1/4]

```C++
muda::HostDeviceConfig::HostDeviceConfig () = default
```




<hr>



### function HostDeviceConfig [2/4]

```C++
inline muda::HostDeviceConfig::HostDeviceConfig (
    const T & value
) 
```




<hr>



### function HostDeviceConfig [3/4]

```C++
muda::HostDeviceConfig::HostDeviceConfig (
    const HostDeviceConfig &
) = default
```




<hr>



### function HostDeviceConfig [4/4]

```C++
muda::HostDeviceConfig::HostDeviceConfig (
    HostDeviceConfig &&
) 
```




<hr>



### function buffer\_view [1/2]

```C++
inline auto muda::HostDeviceConfig::buffer_view () 
```




<hr>



### function buffer\_view [2/2]

```C++
inline auto muda::HostDeviceConfig::buffer_view () const
```




<hr>



### function device\_data 

```C++
inline const T * muda::HostDeviceConfig::device_data () const
```




<hr>



### function host\_data [1/2]

```C++
inline const T * muda::HostDeviceConfig::host_data () const
```




<hr>



### function host\_data [2/2]

```C++
inline T * muda::HostDeviceConfig::host_data () 
```




<hr>



### function operator= 

```C++
HostDeviceConfig & muda::HostDeviceConfig::operator= (
    const HostDeviceConfig < T > &
) = default
```




<hr>



### function operator= 

```C++
HostDeviceConfig & muda::HostDeviceConfig::operator= (
    HostDeviceConfig < T > &&
) = default
```




<hr>



### function operator= 

```C++
inline HostDeviceConfig & muda::HostDeviceConfig::operator= (
    const T & val
) 
```




<hr>



### function view 

```C++
inline auto muda::HostDeviceConfig::view () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/host_device_config.h`

