

# Class muda::details::TempBuffer

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**TempBuffer**](#function-tempbuffer-15) () <br> |
|   | [**TempBuffer**](#function-tempbuffer-25) (size\_t size) <br> |
|   | [**TempBuffer**](#function-tempbuffer-35) ([**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) && other) noexcept<br> |
|   | [**TempBuffer**](#function-tempbuffer-45) (const [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) &) noexcept<br> |
|   | [**TempBuffer**](#function-tempbuffer-55) (const std::vector&lt; T &gt; & vec) <br> |
|  auto | [**capacity**](#function-capacity) () noexcept const<br> |
|  void | [**copy\_from**](#function-copy_from-12) ([**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md)&lt; T &gt; & other, cudaStream\_t stream=nullptr) <br> |
|  void | [**copy\_from**](#function-copy_from-22) (const std::vector&lt; T &gt; & vec, cudaStream\_t stream=nullptr) <br> |
|  void | [**copy\_to**](#function-copy_to) (std::vector&lt; T &gt; & vec, cudaStream\_t stream=nullptr) const<br> |
|  auto | [**data**](#function-data) () noexcept const<br> |
|  void | [**free**](#function-free) () noexcept<br> |
|  [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) & | [**operator=**](#function-operator) ([**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) && other) noexcept<br> |
|  [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) & | [**operator=**](#function-operator_1) (const [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) &) noexcept<br> |
|  [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) & | [**operator=**](#function-operator_2) (const std::vector&lt; T &gt; & vec) <br> |
|  void | [**reserve**](#function-reserve) (size\_t new\_cap, cudaStream\_t stream=nullptr) <br> |
|  void | [**resize**](#function-resize) (size\_t size, cudaStream\_t stream=nullptr) <br> |
|  auto | [**size**](#function-size) () noexcept const<br> |
|   | [**~TempBuffer**](#function-tempbuffer) () <br> |




























## Public Functions Documentation




### function TempBuffer [1/5]

```C++
inline muda::details::TempBuffer::TempBuffer () 
```




<hr>



### function TempBuffer [2/5]

```C++
inline muda::details::TempBuffer::TempBuffer (
    size_t size
) 
```




<hr>



### function TempBuffer [3/5]

```C++
inline muda::details::TempBuffer::TempBuffer (
    TempBuffer && other
) noexcept
```




<hr>



### function TempBuffer [4/5]

```C++
inline muda::details::TempBuffer::TempBuffer (
    const TempBuffer &
) noexcept
```




<hr>



### function TempBuffer [5/5]

```C++
inline muda::details::TempBuffer::TempBuffer (
    const std::vector< T > & vec
) 
```




<hr>



### function capacity 

```C++
inline auto muda::details::TempBuffer::capacity () noexcept const
```




<hr>



### function copy\_from [1/2]

```C++
inline void muda::details::TempBuffer::copy_from (
    TempBuffer < T > & other,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function copy\_from [2/2]

```C++
inline void muda::details::TempBuffer::copy_from (
    const std::vector< T > & vec,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function copy\_to 

```C++
inline void muda::details::TempBuffer::copy_to (
    std::vector< T > & vec,
    cudaStream_t stream=nullptr
) const
```




<hr>



### function data 

```C++
inline auto muda::details::TempBuffer::data () noexcept const
```




<hr>



### function free 

```C++
inline void muda::details::TempBuffer::free () noexcept
```




<hr>



### function operator= 

```C++
inline TempBuffer & muda::details::TempBuffer::operator= (
    TempBuffer && other
) noexcept
```




<hr>



### function operator= 

```C++
inline TempBuffer & muda::details::TempBuffer::operator= (
    const TempBuffer &
) noexcept
```




<hr>



### function operator= 

```C++
inline TempBuffer & muda::details::TempBuffer::operator= (
    const std::vector< T > & vec
) 
```




<hr>



### function reserve 

```C++
inline void muda::details::TempBuffer::reserve (
    size_t new_cap,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function resize 

```C++
inline void muda::details::TempBuffer::resize (
    size_t size,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function size 

```C++
inline auto muda::details::TempBuffer::size () noexcept const
```




<hr>



### function ~TempBuffer 

```C++
inline muda::details::TempBuffer::~TempBuffer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/temp_buffer.h`

