

# Class muda::Logger



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Logger**](classmuda_1_1_logger.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Logger**](#function-logger-14) ([**LoggerViewer**](classmuda_1_1_logger_viewer.md) \* global\_viewer, size\_t meta\_size=DEFAULT\_META\_SIZE, size\_t buffer\_size=DEFAULT\_BUFFER\_SIZE) <br> |
|   | [**Logger**](#function-logger-24) (size\_t meta\_size=DEFAULT\_META\_SIZE, size\_t buffer\_size=DEFAULT\_BUFFER\_SIZE) <br> |
|   | [**Logger**](#function-logger-34) (const [**Logger**](classmuda_1_1_logger.md) &) = delete<br> |
|   | [**Logger**](#function-logger-44) ([**Logger**](classmuda_1_1_logger.md) &&) noexcept<br> |
|  MUDA\_NODISCARD bool | [**is\_buffer\_full**](#function-is_buffer_full) () const<br> |
|  MUDA\_NODISCARD bool | [**is\_meta\_data\_full**](#function-is_meta_data_full) () const<br> |
|  [**Logger**](classmuda_1_1_logger.md) & | [**operator=**](#function-operator) (const [**Logger**](classmuda_1_1_logger.md) &) = delete<br> |
|  [**Logger**](classmuda_1_1_logger.md) & | [**operator=**](#function-operator_1) ([**Logger**](classmuda_1_1_logger.md) &&) noexcept<br> |
|  void | [**retrieve**](#function-retrieve) (std::ostream & o=std::cout) <br> |
|  MUDA\_NODISCARD [**LoggerDataContainer**](classmuda_1_1_logger_data_container.md) | [**retrieve\_meta**](#function-retrieve_meta) () <br> |
|  MUDA\_NODISCARD [**LoggerViewer**](classmuda_1_1_logger_viewer.md) | [**viewer**](#function-viewer) () const<br> |
|   | [**~Logger**](#function-logger) () <br> |




























## Public Functions Documentation




### function Logger [1/4]

```C++
muda::Logger::Logger (
    LoggerViewer * global_viewer,
    size_t meta_size=DEFAULT_META_SIZE,
    size_t buffer_size=DEFAULT_BUFFER_SIZE
) 
```




<hr>



### function Logger [2/4]

```C++
inline muda::Logger::Logger (
    size_t meta_size=DEFAULT_META_SIZE,
    size_t buffer_size=DEFAULT_BUFFER_SIZE
) 
```




<hr>



### function Logger [3/4]

```C++
muda::Logger::Logger (
    const Logger &
) = delete
```




<hr>



### function Logger [4/4]

```C++
muda::Logger::Logger (
    Logger &&
) noexcept
```




<hr>



### function is\_buffer\_full 

```C++
inline MUDA_NODISCARD bool muda::Logger::is_buffer_full () const
```




<hr>



### function is\_meta\_data\_full 

```C++
inline MUDA_NODISCARD bool muda::Logger::is_meta_data_full () const
```




<hr>



### function operator= 

```C++
Logger & muda::Logger::operator= (
    const Logger &
) = delete
```




<hr>



### function operator= 

```C++
Logger & muda::Logger::operator= (
    Logger &&
) noexcept
```




<hr>



### function retrieve 

```C++
void muda::Logger::retrieve (
    std::ostream & o=std::cout
) 
```




<hr>



### function retrieve\_meta 

```C++
MUDA_NODISCARD LoggerDataContainer muda::Logger::retrieve_meta () 
```




<hr>



### function viewer 

```C++
inline MUDA_NODISCARD LoggerViewer muda::Logger::viewer () const
```




<hr>



### function ~Logger 

```C++
muda::Logger::~Logger () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/logger/logger.h`

