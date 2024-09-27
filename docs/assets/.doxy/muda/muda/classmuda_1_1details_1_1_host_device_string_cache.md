

# Class muda::details::HostDeviceStringCache



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**HostDeviceStringCache**](#function-hostdevicestringcache-13) (size\_t buffer\_size=4\_M) <br> |
|   | [**HostDeviceStringCache**](#function-hostdevicestringcache-23) (const [**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) &) = delete<br> |
|   | [**HostDeviceStringCache**](#function-hostdevicestringcache-33) ([**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) &&) = default<br> |
|  [**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) & | [**operator=**](#function-operator) (const [**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) &) = delete<br> |
|  [**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) & | [**operator=**](#function-operator_1) ([**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) &&) = default<br> |
|  [**StringPointer**](classmuda_1_1details_1_1_string_pointer.md) | [**operator[]**](#function-operator_2) (std::string\_view s) <br> |
|   | [**~HostDeviceStringCache**](#function-hostdevicestringcache) () <br> |




























## Public Functions Documentation




### function HostDeviceStringCache [1/3]

```C++
inline muda::details::HostDeviceStringCache::HostDeviceStringCache (
    size_t buffer_size=4_M
) 
```




<hr>



### function HostDeviceStringCache [2/3]

```C++
muda::details::HostDeviceStringCache::HostDeviceStringCache (
    const HostDeviceStringCache &
) = delete
```




<hr>



### function HostDeviceStringCache [3/3]

```C++
muda::details::HostDeviceStringCache::HostDeviceStringCache (
    HostDeviceStringCache &&
) = default
```




<hr>



### function operator= 

```C++
HostDeviceStringCache & muda::details::HostDeviceStringCache::operator= (
    const HostDeviceStringCache &
) = delete
```




<hr>



### function operator= 

```C++
HostDeviceStringCache & muda::details::HostDeviceStringCache::operator= (
    HostDeviceStringCache &&
) = default
```




<hr>



### function operator[] 

```C++
inline StringPointer muda::details::HostDeviceStringCache::operator[] (
    std::string_view s
) 
```




<hr>



### function ~HostDeviceStringCache 

```C++
inline muda::details::HostDeviceStringCache::~HostDeviceStringCache () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/host_device_string_cache.h`

