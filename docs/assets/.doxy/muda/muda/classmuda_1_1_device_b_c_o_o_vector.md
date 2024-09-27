

# Class muda::DeviceBCOOVector

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)








Inherits the following classes: [muda::DeviceDoubletVector](classmuda_1_1_device_doublet_vector.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; T, N, 1 &gt; | [**SegmentVector**](#typedef-segmentvector)  <br> |


## Public Types inherited from muda::DeviceDoubletVector

See [muda::DeviceDoubletVector](classmuda_1_1_device_doublet_vector.md)

| Type | Name |
| ---: | :--- |
| typedef Eigen::Vector&lt; T, N &gt; | [**SegmentVector**](classmuda_1_1_device_doublet_vector.md#typedef-segmentvector)  <br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBCOOVector**](#function-devicebcoovector-13) () = default<br> |
|   | [**DeviceBCOOVector**](#function-devicebcoovector-23) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) &) = default<br> |
|   | [**DeviceBCOOVector**](#function-devicebcoovector-33) ([**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) &&) = default<br> |
|  auto | [**non\_zero\_segments**](#function-non_zero_segments) () const<br> |
|  [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) & | [**operator=**](#function-operator) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) &) = default<br> |
|  [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) & | [**operator=**](#function-operator_1) ([**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) &&) = default<br> |
|   | [**~DeviceBCOOVector**](#function-devicebcoovector) () = default<br> |


## Public Functions inherited from muda::DeviceDoubletVector

See [muda::DeviceDoubletVector](classmuda_1_1_device_doublet_vector.md)

| Type | Name |
| ---: | :--- |
|   | [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md#function-devicedoubletvector) () = default<br> |
|  void | [**clear**](classmuda_1_1_device_doublet_vector.md#function-clear) () <br> |
|  auto | [**doublet\_capacity**](classmuda_1_1_device_doublet_vector.md#function-doublet_capacity) () const<br> |
|  auto | [**doublet\_count**](classmuda_1_1_device_doublet_vector.md#function-doublet_count) () const<br> |
|  void | [**reserve\_doublets**](classmuda_1_1_device_doublet_vector.md#function-reserve_doublets) (size\_t nonzero\_count) <br> |
|  void | [**reshape**](classmuda_1_1_device_doublet_vector.md#function-reshape) (int num\_segment) <br> |
|  void | [**resize**](classmuda_1_1_device_doublet_vector.md#function-resize) (int num\_segment, size\_t nonzero\_count) <br> |
|  void | [**resize\_doublets**](classmuda_1_1_device_doublet_vector.md#function-resize_doublets) (size\_t nonzero\_count) <br> |
|  auto | [**segment\_count**](classmuda_1_1_device_doublet_vector.md#function-segment_count) () const<br> |
|  auto | [**segment\_indices**](classmuda_1_1_device_doublet_vector.md#function-segment_indices-12) () <br> |
|  auto | [**segment\_indices**](classmuda_1_1_device_doublet_vector.md#function-segment_indices-22) () const<br> |
|  auto | [**segment\_values**](classmuda_1_1_device_doublet_vector.md#function-segment_values-12) () <br> |
|  auto | [**segment\_values**](classmuda_1_1_device_doublet_vector.md#function-segment_values-22) () const<br> |
|  auto | [**view**](classmuda_1_1_device_doublet_vector.md#function-view-12) () <br> |
|  auto | [**view**](classmuda_1_1_device_doublet_vector.md#function-view-22) () const<br> |
|  auto | [**viewer**](classmuda_1_1_device_doublet_vector.md#function-viewer-12) () <br> |
|  auto | [**viewer**](classmuda_1_1_device_doublet_vector.md#function-viewer-22) () const<br> |
|   | [**~DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md#function-devicedoubletvector) () = default<br> |
















## Protected Attributes inherited from muda::DeviceDoubletVector

See [muda::DeviceDoubletVector](classmuda_1_1_device_doublet_vector.md)

| Type | Name |
| ---: | :--- |
|  int | [**m\_segment\_count**](classmuda_1_1_device_doublet_vector.md#variable-m_segment_count)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_segment\_indices**](classmuda_1_1_device_doublet_vector.md#variable-m_segment_indices)  <br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; SegmentVector &gt; | [**m\_segment\_values**](classmuda_1_1_device_doublet_vector.md#variable-m_segment_values)  <br> |






































## Public Types Documentation




### typedef SegmentVector 

```C++
using muda::DeviceBCOOVector< T, N >::SegmentVector =  Eigen::Matrix<T, N, 1>;
```




<hr>
## Public Functions Documentation




### function DeviceBCOOVector [1/3]

```C++
muda::DeviceBCOOVector::DeviceBCOOVector () = default
```




<hr>



### function DeviceBCOOVector [2/3]

```C++
muda::DeviceBCOOVector::DeviceBCOOVector (
    const DeviceBCOOVector &
) = default
```




<hr>



### function DeviceBCOOVector [3/3]

```C++
muda::DeviceBCOOVector::DeviceBCOOVector (
    DeviceBCOOVector &&
) = default
```




<hr>



### function non\_zero\_segments 

```C++
inline auto muda::DeviceBCOOVector::non_zero_segments () const
```




<hr>



### function operator= 

```C++
DeviceBCOOVector & muda::DeviceBCOOVector::operator= (
    const DeviceBCOOVector &
) = default
```




<hr>



### function operator= 

```C++
DeviceBCOOVector & muda::DeviceBCOOVector::operator= (
    DeviceBCOOVector &&
) = default
```




<hr>



### function ~DeviceBCOOVector 

```C++
muda::DeviceBCOOVector::~DeviceBCOOVector () = default
```




<hr>## Friends Documentation





### friend MatrixFormatConverter&lt; T, N &gt; 

```C++
class muda::DeviceBCOOVector::MatrixFormatConverter< T, N > (
    details::MatrixFormatConverter < T, N >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_bcoo_vector.h`

