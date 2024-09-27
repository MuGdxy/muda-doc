

# Class muda::LogProxy



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**LogProxy**](classmuda_1_1_log_proxy.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_DEVICE | [**LogProxy**](#function-logproxy-13) () = default<br> |
|  MUDA\_DEVICE | [**LogProxy**](#function-logproxy-23) ([**LoggerViewer**](classmuda_1_1_logger_viewer.md) & viewer) <br> |
|  MUDA\_DEVICE | [**LogProxy**](#function-logproxy-33) (const [**LogProxy**](classmuda_1_1_log_proxy.md) & other) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-110) (Int8, int8\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-210) (Int16, int16\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-310) (Int32, int32\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-410) (Int64, int64\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-510) (UInt8, uint8\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-610) (UInt16, uint16\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-710) (UInt32, uint32\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-810) (UInt64, uint64\_t) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-910) (Float, float) <br> |
|   | [**PROXY\_OPERATOR**](#function-proxy_operator-1010) (Double, double) <br> |
|  MUDA\_DEVICE [**LogProxy**](classmuda_1_1_log_proxy.md) & | [**operator&lt;&lt;**](#function-operator) (const char \* str) <br> |
|  MUDA\_DEVICE bool | [**push\_data**](#function-push_data) (const [**details::LoggerMetaData**](classmuda_1_1details_1_1_logger_meta_data.md) & meta, const void \* data) <br> |
|  MUDA\_DEVICE void | [**push\_fmt\_arg**](#function-push_fmt_arg) (const T & obj, LoggerFmtArg fmt\_arg\_func) <br> |
|  MUDA\_DEVICE [**LogProxy**](classmuda_1_1_log_proxy.md) & | [**push\_string**](#function-push_string) (const char \* str) <br> |




























## Public Functions Documentation




### function LogProxy [1/3]

```C++
MUDA_DEVICE muda::LogProxy::LogProxy () = default
```




<hr>



### function LogProxy [2/3]

```C++
MUDA_DEVICE muda::LogProxy::LogProxy (
    LoggerViewer & viewer
) 
```




<hr>



### function LogProxy [3/3]

```C++
inline MUDA_DEVICE muda::LogProxy::LogProxy (
    const LogProxy & other
) 
```




<hr>



### function PROXY\_OPERATOR [1/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    Int8,
    int8_t
) 
```




<hr>



### function PROXY\_OPERATOR [2/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    Int16,
    int16_t
) 
```




<hr>



### function PROXY\_OPERATOR [3/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    Int32,
    int32_t
) 
```




<hr>



### function PROXY\_OPERATOR [4/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    Int64,
    int64_t
) 
```




<hr>



### function PROXY\_OPERATOR [5/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    UInt8,
    uint8_t
) 
```




<hr>



### function PROXY\_OPERATOR [6/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    UInt16,
    uint16_t
) 
```




<hr>



### function PROXY\_OPERATOR [7/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    UInt32,
    uint32_t
) 
```




<hr>



### function PROXY\_OPERATOR [8/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    UInt64,
    uint64_t
) 
```




<hr>



### function PROXY\_OPERATOR [9/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    Float,
    float
) 
```




<hr>



### function PROXY\_OPERATOR [10/10]

```C++
muda::LogProxy::PROXY_OPERATOR (
    Double,
    double
) 
```




<hr>



### function operator&lt;&lt; 

```C++
MUDA_DEVICE LogProxy & muda::LogProxy::operator<< (
    const char * str
) 
```




<hr>



### function push\_data 

```C++
MUDA_DEVICE bool muda::LogProxy::push_data (
    const details::LoggerMetaData & meta,
    const void * data
) 
```




<hr>



### function push\_fmt\_arg 

```C++
template<typename T>
MUDA_DEVICE void muda::LogProxy::push_fmt_arg (
    const T & obj,
    LoggerFmtArg fmt_arg_func
) 
```




<hr>



### function push\_string 

```C++
template<bool IsFmt>
MUDA_DEVICE LogProxy & muda::LogProxy::push_string (
    const char * str
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/logger/logger_viewer.h`

