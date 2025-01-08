

# Class muda::DeviceBuffer3D

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBuffer3D**](#function-devicebuffer3d-15) (const [**Extent3D**](classmuda_1_1_extent3_d.md) & n) <br> |
|   | [**DeviceBuffer3D**](#function-devicebuffer3d-25) () <br> |
|   | [**DeviceBuffer3D**](#function-devicebuffer3d-35) (const [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & other) <br> |
|   | [**DeviceBuffer3D**](#function-devicebuffer3d-45) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md) && other) <br> |
|   | [**DeviceBuffer3D**](#function-devicebuffer3d-55) ([**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; other) <br> |
|  auto | [**capacity**](#function-capacity) () const<br> |
|  void | [**clear**](#function-clear) () <br> |
|  void | [**copy\_from**](#function-copy_from) (const std::vector&lt; T &gt; & host) <br> |
|  void | [**copy\_to**](#function-copy_to) (std::vector&lt; T &gt; & host) const<br> |
|  [**CDense3D**](classmuda_1_1_dense3_d_base.md)&lt; T &gt; | [**cviewer**](#function-cviewer) () const<br> |
|  T \* | [**data**](#function-data-12) () <br> |
|  const T \* | [**data**](#function-data-22) () const<br> |
|  auto | [**extent**](#function-extent) () const<br> |
|  void | [**fill**](#function-fill) (const T & v) <br> |
|   | [**operator Buffer3DView&lt; T &gt;**](#function-operator-buffer3dview<-t->) () <br> |
|   | [**operator CBuffer3DView&lt; T &gt;**](#function-operator-cbuffer3dview<-t->) () const<br> |
|  [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md) & | [**operator=**](#function-operator) (const [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & other) <br> |
|  [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md) & | [**operator=**](#function-operator_1) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; && other) <br> |
|  [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md) & | [**operator=**](#function-operator_2) ([**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; other) <br> |
|  auto | [**pitch\_bytes**](#function-pitch_bytes) () const<br> |
|  auto | [**pitch\_bytes\_area**](#function-pitch_bytes_area) () const<br> |
|  void | [**reserve**](#function-reserve) ([**Extent3D**](classmuda_1_1_extent3_d.md) new\_capacity) <br> |
|  void | [**resize**](#function-resize-12) ([**Extent3D**](classmuda_1_1_extent3_d.md) new\_size) <br> |
|  void | [**resize**](#function-resize-22) ([**Extent3D**](classmuda_1_1_extent3_d.md) new\_size, const T & value) <br> |
|  void | [**shrink\_to\_fit**](#function-shrink_to_fit) () <br> |
|  auto | [**total\_size**](#function-total_size) () const<br> |
|  [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; | [**view**](#function-view-14) ([**Offset3D**](classmuda_1_1_offset3_d.md) offset, [**Extent3D**](classmuda_1_1_extent3_d.md) extent={}) <br> |
|  [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; | [**view**](#function-view-24) () <br> |
|  [**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; | [**view**](#function-view-34) ([**Offset3D**](classmuda_1_1_offset3_d.md) offset, [**Extent3D**](classmuda_1_1_extent3_d.md) extent={}) const<br> |
|  [**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; | [**view**](#function-view-44) () const<br> |
|  [**Dense3D**](classmuda_1_1_dense3_d_base.md)&lt; T &gt; | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceBuffer3D**](#function-devicebuffer3d) () <br> |




























## Public Types Documentation




### typedef value\_type 

```C++
using muda::DeviceBuffer3D< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function DeviceBuffer3D [1/5]

```C++
muda::DeviceBuffer3D::DeviceBuffer3D (
    const Extent3D & n
) 
```




<hr>



### function DeviceBuffer3D [2/5]

```C++
muda::DeviceBuffer3D::DeviceBuffer3D () 
```




<hr>



### function DeviceBuffer3D [3/5]

```C++
muda::DeviceBuffer3D::DeviceBuffer3D (
    const DeviceBuffer3D < T > & other
) 
```




<hr>



### function DeviceBuffer3D [4/5]

```C++
muda::DeviceBuffer3D::DeviceBuffer3D (
    DeviceBuffer3D && other
) 
```




<hr>



### function DeviceBuffer3D [5/5]

```C++
muda::DeviceBuffer3D::DeviceBuffer3D (
    CBuffer3DView < T > other
) 
```




<hr>



### function capacity 

```C++
inline auto muda::DeviceBuffer3D::capacity () const
```




<hr>



### function clear 

```C++
void muda::DeviceBuffer3D::clear () 
```




<hr>



### function copy\_from 

```C++
void muda::DeviceBuffer3D::copy_from (
    const std::vector< T > & host
) 
```




<hr>



### function copy\_to 

```C++
void muda::DeviceBuffer3D::copy_to (
    std::vector< T > & host
) const
```




<hr>



### function cviewer 

```C++
inline CDense3D < T > muda::DeviceBuffer3D::cviewer () const
```




<hr>



### function data [1/2]

```C++
inline T * muda::DeviceBuffer3D::data () 
```




<hr>



### function data [2/2]

```C++
inline const T * muda::DeviceBuffer3D::data () const
```




<hr>



### function extent 

```C++
inline auto muda::DeviceBuffer3D::extent () const
```




<hr>



### function fill 

```C++
void muda::DeviceBuffer3D::fill (
    const T & v
) 
```




<hr>



### function operator Buffer3DView&lt; T &gt; 

```C++
inline muda::DeviceBuffer3D::operator Buffer3DView< T > () 
```




<hr>



### function operator CBuffer3DView&lt; T &gt; 

```C++
inline muda::DeviceBuffer3D::operator CBuffer3DView< T > () const
```




<hr>



### function operator= 

```C++
DeviceBuffer3D & muda::DeviceBuffer3D::operator= (
    const DeviceBuffer3D < T > & other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer3D & muda::DeviceBuffer3D::operator= (
    DeviceBuffer3D < T > && other
) 
```




<hr>



### function operator= 

```C++
DeviceBuffer3D & muda::DeviceBuffer3D::operator= (
    CBuffer3DView < T > other
) 
```




<hr>



### function pitch\_bytes 

```C++
inline auto muda::DeviceBuffer3D::pitch_bytes () const
```




<hr>



### function pitch\_bytes\_area 

```C++
inline auto muda::DeviceBuffer3D::pitch_bytes_area () const
```




<hr>



### function reserve 

```C++
void muda::DeviceBuffer3D::reserve (
    Extent3D new_capacity
) 
```




<hr>



### function resize [1/2]

```C++
void muda::DeviceBuffer3D::resize (
    Extent3D new_size
) 
```




<hr>



### function resize [2/2]

```C++
void muda::DeviceBuffer3D::resize (
    Extent3D new_size,
    const T & value
) 
```




<hr>



### function shrink\_to\_fit 

```C++
void muda::DeviceBuffer3D::shrink_to_fit () 
```




<hr>



### function total\_size 

```C++
inline auto muda::DeviceBuffer3D::total_size () const
```




<hr>



### function view [1/4]

```C++
inline Buffer3DView < T > muda::DeviceBuffer3D::view (
    Offset3D offset,
    Extent3D extent={}
) 
```




<hr>



### function view [2/4]

```C++
inline Buffer3DView < T > muda::DeviceBuffer3D::view () 
```




<hr>



### function view [3/4]

```C++
inline CBuffer3DView < T > muda::DeviceBuffer3D::view (
    Offset3D offset,
    Extent3D extent={}
) const
```




<hr>



### function view [4/4]

```C++
inline CBuffer3DView < T > muda::DeviceBuffer3D::view () const
```




<hr>



### function viewer 

```C++
inline Dense3D < T > muda::DeviceBuffer3D::viewer () 
```




<hr>



### function ~DeviceBuffer3D 

```C++
muda::DeviceBuffer3D::~DeviceBuffer3D () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/buffer_fwd.h`

