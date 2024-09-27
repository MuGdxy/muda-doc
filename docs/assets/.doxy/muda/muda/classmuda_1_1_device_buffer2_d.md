

# Class muda::DeviceBuffer2D

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBuffer2D**](#function-devicebuffer2d-15) (const [**Extent2D**](classmuda_1_1_extent2_d.md) & n) <br> |
|   | [**DeviceBuffer2D**](#function-devicebuffer2d-25) () <br> |
|   | [**DeviceBuffer2D**](#function-devicebuffer2d-35) (const [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & other) <br> |
|   | [**DeviceBuffer2D**](#function-devicebuffer2d-45) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md) && other) <br> |
|   | [**DeviceBuffer2D**](#function-devicebuffer2d-55) ([**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; other) <br> |
|  auto | [**capacity**](#function-capacity) () const<br> |
|  void | [**clear**](#function-clear) () <br> |
|  void | [**copy\_from**](#function-copy_from) (const std::vector&lt; T &gt; & host) <br> |
|  void | [**copy\_to**](#function-copy_to) (std::vector&lt; T &gt; & host) const<br> |
|  [**CDense2D**](classmuda_1_1_dense2_d_base.md)&lt; T &gt; | [**cviewer**](#function-cviewer) () const<br> |
|  T \* | [**data**](#function-data-12) () <br> |
|  const T \* | [**data**](#function-data-22) () const<br> |
|  auto | [**extent**](#function-extent) () const<br> |
|  void | [**fill**](#function-fill) (const T & v) <br> |
|   | [**operator Buffer2DView&lt; T &gt;**](#function-operator-buffer2dview<-t->) () <br> |
|   | [**operator CBuffer2DView&lt; T &gt;**](#function-operator-cbuffer2dview<-t->) () const<br> |
|  [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md) & | [**operator=**](#function-operator) (const [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & other) <br> |
|  [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md) & | [**operator=**](#function-operator_1) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; && other) <br> |
|  [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md) & | [**operator=**](#function-operator_2) ([**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; other) <br> |
|  auto | [**pitch\_bytes**](#function-pitch_bytes) () const<br> |
|  void | [**reserve**](#function-reserve) ([**Extent2D**](classmuda_1_1_extent2_d.md) new\_capacity) <br> |
|  void | [**resize**](#function-resize-12) ([**Extent2D**](classmuda_1_1_extent2_d.md) new\_extent) <br> |
|  void | [**resize**](#function-resize-22) ([**Extent2D**](classmuda_1_1_extent2_d.md) new\_extent, const T & value) <br> |
|  void | [**shrink\_to\_fit**](#function-shrink_to_fit) () <br> |
|  auto | [**total\_size**](#function-total_size) () const<br> |
|  [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; | [**view**](#function-view-14) ([**Offset2D**](classmuda_1_1_offset2_d.md) offset, [**Extent2D**](classmuda_1_1_extent2_d.md) extent={}) <br> |
|  [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; | [**view**](#function-view-24) () <br> |
|  [**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; | [**view**](#function-view-34) ([**Offset2D**](classmuda_1_1_offset2_d.md) offset, [**Extent2D**](classmuda_1_1_extent2_d.md) extent={}) const<br> |
|  [**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; | [**view**](#function-view-44) () const<br> |
|  [**Dense2D**](classmuda_1_1_dense2_d_base.md)&lt; T &gt; | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceBuffer2D**](#function-devicebuffer2d) () <br> |




























## Public Types Documentation




### typedef value\_type 

```C++
using muda::DeviceBuffer2D< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function DeviceBuffer2D [1/5]

```C++
muda::DeviceBuffer2D::DeviceBuffer2D (
    const Extent2D & n
) 
```




<hr>



### function DeviceBuffer2D [2/5]

```C++
muda::DeviceBuffer2D::DeviceBuffer2D () 
```




<hr>



### function DeviceBuffer2D [3/5]

```C++
muda::DeviceBuffer2D::DeviceBuffer2D (
    const DeviceBuffer2D < T > & other
) 
```




<hr>



### function DeviceBuffer2D [4/5]

```C++
muda::DeviceBuffer2D::DeviceBuffer2D (
    DeviceBuffer2D && other
) 
```




<hr>



### function DeviceBuffer2D [5/5]

```C++
muda::DeviceBuffer2D::DeviceBuffer2D (
    CBuffer2DView < T > other
) 
```




<hr>



### function capacity 

```C++
inline auto muda::DeviceBuffer2D::capacity () const
```




<hr>



### function clear 

```C++
void muda::DeviceBuffer2D::clear () 
```




<hr>



### function copy\_from 

```C++
void muda::DeviceBuffer2D::copy_from (
    const std::vector< T > & host
) 
```




<hr>



### function copy\_to 

```C++
void muda::DeviceBuffer2D::copy_to (
    std::vector< T > & host
) const
```




<hr>



### function cviewer 

```C++
inline CDense2D < T > muda::DeviceBuffer2D::cviewer () const
```




<hr>



### function data [1/2]

```C++
inline T * muda::DeviceBuffer2D::data () 
```




<hr>



### function data [2/2]

```C++
inline const T * muda::DeviceBuffer2D::data () const
```




<hr>



### function extent 

```C++
inline auto muda::DeviceBuffer2D::extent () const
```




<hr>



### function fill 

```C++
void muda::DeviceBuffer2D::fill (
    const T & v
) 
```




<hr>



### function operator Buffer2DView&lt; T &gt; 

```C++
inline muda::DeviceBuffer2D::operator Buffer2DView< T > () 
```




<hr>



### function operator CBuffer2DView&lt; T &gt; 

```C++
inline muda::DeviceBuffer2D::operator CBuffer2DView< T > () const
```




<hr>



### function operator= 

```C++
DeviceBuffer2D & muda::DeviceBuffer2D::operator= (
    const DeviceBuffer2D < T > & other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer2D & muda::DeviceBuffer2D::operator= (
    DeviceBuffer2D < T > && other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer2D & muda::DeviceBuffer2D::operator= (
    CBuffer2DView < T > other
) 
```




<hr>



### function pitch\_bytes 

```C++
inline auto muda::DeviceBuffer2D::pitch_bytes () const
```




<hr>



### function reserve 

```C++
void muda::DeviceBuffer2D::reserve (
    Extent2D new_capacity
) 
```




<hr>



### function resize [1/2]

```C++
void muda::DeviceBuffer2D::resize (
    Extent2D new_extent
) 
```




<hr>



### function resize [2/2]

```C++
void muda::DeviceBuffer2D::resize (
    Extent2D new_extent,
    const T & value
) 
```




<hr>



### function shrink\_to\_fit 

```C++
void muda::DeviceBuffer2D::shrink_to_fit () 
```




<hr>



### function total\_size 

```C++
inline auto muda::DeviceBuffer2D::total_size () const
```




<hr>



### function view [1/4]

```C++
inline Buffer2DView < T > muda::DeviceBuffer2D::view (
    Offset2D offset,
    Extent2D extent={}
) 
```




<hr>



### function view [2/4]

```C++
inline Buffer2DView < T > muda::DeviceBuffer2D::view () 
```




<hr>



### function view [3/4]

```C++
inline CBuffer2DView < T > muda::DeviceBuffer2D::view (
    Offset2D offset,
    Extent2D extent={}
) const
```




<hr>



### function view [4/4]

```C++
inline CBuffer2DView < T > muda::DeviceBuffer2D::view () const
```




<hr>



### function viewer 

```C++
inline Dense2D < T > muda::DeviceBuffer2D::viewer () 
```




<hr>



### function ~DeviceBuffer2D 

```C++
muda::DeviceBuffer2D::~DeviceBuffer2D () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/device_buffer_2d.h`

