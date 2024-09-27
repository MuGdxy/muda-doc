

# Class muda::DeviceDoubletVector

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)










Inherited by the following classes: [muda::DeviceBCOOVector](classmuda_1_1_device_b_c_o_o_vector.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Vector&lt; T, N &gt; | [**SegmentVector**](#typedef-segmentvector)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceDoubletVector**](#function-devicedoubletvector) () = default<br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**doublet\_capacity**](#function-doublet_capacity) () const<br> |
|  auto | [**doublet\_count**](#function-doublet_count) () const<br> |
|  void | [**reserve\_doublets**](#function-reserve_doublets) (size\_t nonzero\_count) <br> |
|  void | [**reshape**](#function-reshape) (int num\_segment) <br> |
|  void | [**resize**](#function-resize) (int num\_segment, size\_t nonzero\_count) <br> |
|  void | [**resize\_doublets**](#function-resize_doublets) (size\_t nonzero\_count) <br> |
|  auto | [**segment\_count**](#function-segment_count) () const<br> |
|  auto | [**segment\_indices**](#function-segment_indices-12) () <br> |
|  auto | [**segment\_indices**](#function-segment_indices-22) () const<br> |
|  auto | [**segment\_values**](#function-segment_values-12) () <br> |
|  auto | [**segment\_values**](#function-segment_values-22) () const<br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|  auto | [**viewer**](#function-viewer-12) () <br> |
|  auto | [**viewer**](#function-viewer-22) () const<br> |
|   | [**~DeviceDoubletVector**](#function-devicedoubletvector) () = default<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_segment\_count**](#variable-m_segment_count)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_segment\_indices**](#variable-m_segment_indices)  <br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; SegmentVector &gt; | [**m\_segment\_values**](#variable-m_segment_values)  <br> |




















## Public Types Documentation




### typedef SegmentVector 

```C++
using muda::DeviceDoubletVector< T, N >::SegmentVector =  Eigen::Vector<T, N>;
```




<hr>
## Public Functions Documentation




### function DeviceDoubletVector 

```C++
muda::DeviceDoubletVector::DeviceDoubletVector () = default
```




<hr>



### function clear 

```C++
inline void muda::DeviceDoubletVector::clear () 
```




<hr>



### function doublet\_capacity 

```C++
inline auto muda::DeviceDoubletVector::doublet_capacity () const
```




<hr>



### function doublet\_count 

```C++
inline auto muda::DeviceDoubletVector::doublet_count () const
```




<hr>



### function reserve\_doublets 

```C++
inline void muda::DeviceDoubletVector::reserve_doublets (
    size_t nonzero_count
) 
```




<hr>



### function reshape 

```C++
inline void muda::DeviceDoubletVector::reshape (
    int num_segment
) 
```




<hr>



### function resize 

```C++
inline void muda::DeviceDoubletVector::resize (
    int num_segment,
    size_t nonzero_count
) 
```




<hr>



### function resize\_doublets 

```C++
inline void muda::DeviceDoubletVector::resize_doublets (
    size_t nonzero_count
) 
```




<hr>



### function segment\_count 

```C++
inline auto muda::DeviceDoubletVector::segment_count () const
```




<hr>



### function segment\_indices [1/2]

```C++
inline auto muda::DeviceDoubletVector::segment_indices () 
```




<hr>



### function segment\_indices [2/2]

```C++
inline auto muda::DeviceDoubletVector::segment_indices () const
```




<hr>



### function segment\_values [1/2]

```C++
inline auto muda::DeviceDoubletVector::segment_values () 
```




<hr>



### function segment\_values [2/2]

```C++
inline auto muda::DeviceDoubletVector::segment_values () const
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceDoubletVector::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceDoubletVector::view () const
```




<hr>



### function viewer [1/2]

```C++
inline auto muda::DeviceDoubletVector::viewer () 
```




<hr>



### function viewer [2/2]

```C++
inline auto muda::DeviceDoubletVector::viewer () const
```




<hr>



### function ~DeviceDoubletVector 

```C++
muda::DeviceDoubletVector::~DeviceDoubletVector () = default
```




<hr>
## Protected Attributes Documentation




### variable m\_segment\_count 

```C++
int muda::DeviceDoubletVector< T, N >::m_segment_count;
```




<hr>



### variable m\_segment\_indices 

```C++
muda::DeviceBuffer<int> muda::DeviceDoubletVector< T, N >::m_segment_indices;
```




<hr>



### variable m\_segment\_values 

```C++
muda::DeviceBuffer<SegmentVector> muda::DeviceDoubletVector< T, N >::m_segment_values;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename U, int M>
class muda::DeviceDoubletVector::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_doublet_vector.h`

