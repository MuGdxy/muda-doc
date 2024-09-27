

# Class muda::Stream



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Stream**](classmuda_1_1_stream.md)



_RAII wrapper for cudaStream._ 

* `#include <stream.h>`















## Classes

| Type | Name |
| ---: | :--- |
| class | [**FireAndForget**](classmuda_1_1_stream_1_1_fire_and_forget.md) <br> |
| class | [**GraphFireAndForget**](classmuda_1_1_stream_1_1_graph_fire_and_forget.md) <br> |
| class | [**GraphTailLaunch**](classmuda_1_1_stream_1_1_graph_tail_launch.md) <br> |
| class | [**TailLaunch**](classmuda_1_1_stream_1_1_tail_launch.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum unsigned int | [**Flag**](#enum-flag)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_NODISCARD | [**Stream**](#function-stream-14) (Flag f=Flag::eDefault) <br> |
|   | [**Stream**](#function-stream-24) (const [**Stream**](classmuda_1_1_stream.md) &) = delete<br> |
|   | [**Stream**](#function-stream-34) ([**Stream**](classmuda_1_1_stream.md) && o) <br> |
|  void | [**begin\_capture**](#function-begin_capture) (cudaStreamCaptureMode mode=cudaStreamCaptureModeThreadLocal) const<br> |
|  void | [**end\_capture**](#function-end_capture) (cudaGraph\_t \* graph) const<br> |
|   | [**operator cudaStream\_t**](#function-operator-cudastream_t) () const<br> |
|  [**Stream**](classmuda_1_1_stream.md) & | [**operator=**](#function-operator) (const [**Stream**](classmuda_1_1_stream.md) &) = delete<br> |
|  [**Stream**](classmuda_1_1_stream.md) & | [**operator=**](#function-operator_1) ([**Stream**](classmuda_1_1_stream.md) && o) <br> |
|  cudaStream\_t | [**view**](#function-view) () const<br> |
|  void | [**wait**](#function-wait) () const<br> |
|  std::byte \* | [**workspace**](#function-workspace) (size\_t byte\_size) <br> |
|   | [**~Stream**](#function-stream) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Stream**](classmuda_1_1_stream.md) & | [**Default**](#function-default) () <br> |


























## Public Types Documentation




### enum Flag 

```C++
enum muda::Stream::Flag {
    eDefault = cudaStreamDefault,
    eNonBlocking = cudaStreamNonBlocking
};
```




<hr>
## Public Functions Documentation




### function Stream [1/4]

```C++
MUDA_NODISCARD muda::Stream::Stream (
    Flag f=Flag::eDefault
) 
```




<hr>



### function Stream [2/4]

```C++
muda::Stream::Stream (
    const Stream &
) = delete
```




<hr>



### function Stream [3/4]

```C++
muda::Stream::Stream (
    Stream && o
) 
```




<hr>



### function begin\_capture 

```C++
void muda::Stream::begin_capture (
    cudaStreamCaptureMode mode=cudaStreamCaptureModeThreadLocal
) const
```




<hr>



### function end\_capture 

```C++
void muda::Stream::end_capture (
    cudaGraph_t * graph
) const
```




<hr>



### function operator cudaStream\_t 

```C++
inline muda::Stream::operator cudaStream_t () const
```




<hr>



### function operator= 

```C++
Stream & muda::Stream::operator= (
    const Stream &
) = delete
```




<hr>



### function operator= 

```C++
Stream & muda::Stream::operator= (
    Stream && o
) 
```




<hr>



### function view 

```C++
inline cudaStream_t muda::Stream::view () const
```




<hr>



### function wait 

```C++
void muda::Stream::wait () const
```




<hr>



### function workspace 

```C++
std::byte * muda::Stream::workspace (
    size_t byte_size
) 
```




<hr>



### function ~Stream 

```C++
muda::Stream::~Stream () 
```




<hr>
## Public Static Functions Documentation




### function Default 

```C++
static Stream & muda::Stream::Default () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/stream.h`

