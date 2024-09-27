

# Class muda::LoggerViewer



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**LoggerViewer**](classmuda_1_1_logger_viewer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**operator bool**](#function-operator-bool) () const<br> |
|  MUDA\_DEVICE [**LogProxy**](classmuda_1_1_log_proxy.md) | [**operator&lt;&lt;**](#function-operator) (const T & t) <br> |
|  MUDA\_DEVICE [**LogProxy**](classmuda_1_1_log_proxy.md) | [**operator&lt;&lt;**](#function-operator_1) (const char \* s) <br> |
|  MUDA\_DEVICE [**LogProxy**](classmuda_1_1_log_proxy.md) | [**proxy**](#function-proxy) () <br> |
|  MUDA\_DEVICE [**LogProxy**](classmuda_1_1_log_proxy.md) | [**push\_string**](#function-push_string) (const char \* str) <br> |




























## Public Functions Documentation




### function operator bool 

```C++
inline MUDA_GENERIC muda::LoggerViewer::operator bool () const
```




<hr>



### function operator&lt;&lt; 

```C++
template<typename T>
MUDA_DEVICE LogProxy muda::LoggerViewer::operator<< (
    const T & t
) 
```




<hr>



### function operator&lt;&lt; 

```C++
MUDA_DEVICE LogProxy muda::LoggerViewer::operator<< (
    const char * s
) 
```




<hr>



### function proxy 

```C++
inline MUDA_DEVICE LogProxy muda::LoggerViewer::proxy () 
```




<hr>



### function push\_string 

```C++
template<bool IsFmt>
MUDA_DEVICE LogProxy muda::LoggerViewer::push_string (
    const char * str
) 
```




<hr>## Friends Documentation





### friend LogProxy 

```C++
class muda::LoggerViewer::LogProxy (
    LogProxy
) 
```




<hr>



### friend Logger 

```C++
class muda::LoggerViewer::Logger (
    Logger
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/logger/logger_viewer.h`

