

# Class muda::DeviceBuffer

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBuffer**](classmuda_1_1_device_buffer.md)



_A_ `std::vector` _like wrapper of cuda device memory, allows user to:_[More...](#detailed-description)

* `#include <device_buffer.h>`

















## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBuffer**](#function-devicebuffer-16) (size\_t n) <br> |
|   | [**DeviceBuffer**](#function-devicebuffer-26) () <br> |
|   | [**DeviceBuffer**](#function-devicebuffer-36) (const [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & other) <br> |
|   | [**DeviceBuffer**](#function-devicebuffer-46) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md) && other) <br> |
|   | [**DeviceBuffer**](#function-devicebuffer-56) ([**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; other) <br> |
|   | [**DeviceBuffer**](#function-devicebuffer-66) (const std::vector&lt; T &gt; & host) <br> |
|  auto | [**capacity**](#function-capacity) () const<br> |
|  void | [**clear**](#function-clear) () <br> |
|  void | [**copy\_from**](#function-copy_from) (const std::vector&lt; T &gt; & host) <br> |
|  void | [**copy\_to**](#function-copy_to) (std::vector&lt; T &gt; & host) const<br> |
|  [**CDense1D**](classmuda_1_1_dense1_d_t.md)&lt; T &gt; | [**cviewer**](#function-cviewer) () const<br> |
|  T \* | [**data**](#function-data-12) () <br> |
|  const T \* | [**data**](#function-data-22) () const<br> |
|  void | [**fill**](#function-fill) (const T & v) <br> |
|   | [**operator BufferView&lt; T &gt;**](#function-operator-bufferview<-t->) () <br> |
|   | [**operator CBufferView&lt; T &gt;**](#function-operator-cbufferview<-t->) () const<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md) & | [**operator=**](#function-operator) (const [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & other) <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md) & | [**operator=**](#function-operator_1) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; && other) <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md) & | [**operator=**](#function-operator_2) ([**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; other) <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md) & | [**operator=**](#function-operator_3) (const std::vector&lt; T &gt; & other) <br> |
|  void | [**reserve**](#function-reserve) (size\_t new\_capacity) <br> |
|  void | [**resize**](#function-resize-12) (size\_t new\_size) <br> |
|  void | [**resize**](#function-resize-22) (size\_t new\_size, const T & value) <br> |
|  void | [**shrink\_to\_fit**](#function-shrink_to_fit) () <br> |
|  auto | [**size**](#function-size) () const<br> |
|  [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; | [**view**](#function-view-14) (size\_t offset, size\_t size=~0) <br> |
|  [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; | [**view**](#function-view-24) () <br> |
|  [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; | [**view**](#function-view-34) (size\_t offset, size\_t size=~0) const<br> |
|  [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; | [**view**](#function-view-44) () const<br> |
|  [**Dense1D**](classmuda_1_1_dense1_d_t.md)&lt; T &gt; | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceBuffer**](#function-devicebuffer) () <br> |




























## Detailed Description



* resize 
* reserve 
* clear 
* fill 
* shrink\_to\_fit 
* make view or subview from it 
* make a safe viewer from it



**See also:** 



    
## Public Types Documentation




### typedef value\_type 

```C++
using muda::DeviceBuffer< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function DeviceBuffer [1/6]

```C++
muda::DeviceBuffer::DeviceBuffer (
    size_t n
) 
```




<hr>



### function DeviceBuffer [2/6]

```C++
muda::DeviceBuffer::DeviceBuffer () 
```




<hr>



### function DeviceBuffer [3/6]

```C++
muda::DeviceBuffer::DeviceBuffer (
    const DeviceBuffer < T > & other
) 
```




<hr>



### function DeviceBuffer [4/6]

```C++
muda::DeviceBuffer::DeviceBuffer (
    DeviceBuffer && other
) 
```




<hr>



### function DeviceBuffer [5/6]

```C++
muda::DeviceBuffer::DeviceBuffer (
    CBufferView < T > other
) 
```




<hr>



### function DeviceBuffer [6/6]

```C++
muda::DeviceBuffer::DeviceBuffer (
    const std::vector< T > & host
) 
```




<hr>



### function capacity 

```C++
inline auto muda::DeviceBuffer::capacity () const
```




<hr>



### function clear 

```C++
void muda::DeviceBuffer::clear () 
```




<hr>



### function copy\_from 

```C++
void muda::DeviceBuffer::copy_from (
    const std::vector< T > & host
) 
```




<hr>



### function copy\_to 

```C++
void muda::DeviceBuffer::copy_to (
    std::vector< T > & host
) const
```




<hr>



### function cviewer 

```C++
CDense1D < T > muda::DeviceBuffer::cviewer () const
```




<hr>



### function data [1/2]

```C++
inline T * muda::DeviceBuffer::data () 
```




<hr>



### function data [2/2]

```C++
inline const T * muda::DeviceBuffer::data () const
```




<hr>



### function fill 

```C++
void muda::DeviceBuffer::fill (
    const T & v
) 
```




<hr>



### function operator BufferView&lt; T &gt; 

```C++
inline muda::DeviceBuffer::operator BufferView< T > () 
```




<hr>



### function operator CBufferView&lt; T &gt; 

```C++
inline muda::DeviceBuffer::operator CBufferView< T > () const
```




<hr>



### function operator= 

```C++
DeviceBuffer & muda::DeviceBuffer::operator= (
    const DeviceBuffer < T > & other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer & muda::DeviceBuffer::operator= (
    DeviceBuffer < T > && other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer & muda::DeviceBuffer::operator= (
    CBufferView < T > other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer & muda::DeviceBuffer::operator= (
    const std::vector< T > & other
) 
```




<hr>



### function reserve 

```C++
void muda::DeviceBuffer::reserve (
    size_t new_capacity
) 
```




<hr>



### function resize [1/2]

```C++
void muda::DeviceBuffer::resize (
    size_t new_size
) 
```




<hr>



### function resize [2/2]

```C++
void muda::DeviceBuffer::resize (
    size_t new_size,
    const T & value
) 
```




<hr>



### function shrink\_to\_fit 

```C++
void muda::DeviceBuffer::shrink_to_fit () 
```




<hr>



### function size 

```C++
inline auto muda::DeviceBuffer::size () const
```




<hr>



### function view [1/4]

```C++
BufferView < T > muda::DeviceBuffer::view (
    size_t offset,
    size_t size=~0
) 
```




<hr>



### function view [2/4]

```C++
BufferView < T > muda::DeviceBuffer::view () 
```




<hr>



### function view [3/4]

```C++
CBufferView < T > muda::DeviceBuffer::view (
    size_t offset,
    size_t size=~0
) const
```




<hr>



### function view [4/4]

```C++
CBufferView < T > muda::DeviceBuffer::view () const
```




<hr>



### function viewer 

```C++
Dense1D < T > muda::DeviceBuffer::viewer () 
```




<hr>



### function ~DeviceBuffer 

```C++
muda::DeviceBuffer::~DeviceBuffer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/device_buffer.h`

