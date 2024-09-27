

# Class muda::cuda\_error

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**cuda\_error**](classmuda_1_1cuda__error.md)








Inherits the following classes: [muda::exception](classmuda_1_1exception.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**cuda\_error**](#function-cuda_error) (T error, std::string error\_string, const std::string & file, size\_t line, const std::string & func) <br> |
|  T | [**error**](#function-error) () const<br> |
|  const std::string & | [**error\_string**](#function-error_string) () const<br> |
|  const std::string & | [**file**](#function-file) () const<br> |
|  const std::string & | [**func**](#function-func) () const<br> |
|  size\_t | [**line**](#function-line) () const<br> |


## Public Functions inherited from muda::exception

See [muda::exception](classmuda_1_1exception.md)

| Type | Name |
| ---: | :--- |
|   | [**exception**](classmuda_1_1exception.md#function-exception) (const std::string & msg) <br> |
| virtual char const \* | [**what**](classmuda_1_1exception.md#function-what) () const<br> |






















































## Public Functions Documentation




### function cuda\_error 

```C++
inline muda::cuda_error::cuda_error (
    T error,
    std::string error_string,
    const std::string & file,
    size_t line,
    const std::string & func
) 
```




<hr>



### function error 

```C++
inline T muda::cuda_error::error () const
```




<hr>



### function error\_string 

```C++
inline const std::string & muda::cuda_error::error_string () const
```




<hr>



### function file 

```C++
inline const std::string & muda::cuda_error::file () const
```




<hr>



### function func 

```C++
inline const std::string & muda::cuda_error::func () const
```




<hr>



### function line 

```C++
inline size_t muda::cuda_error::line () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/check/check.h`

