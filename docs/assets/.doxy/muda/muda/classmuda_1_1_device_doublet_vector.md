

# Class muda::DeviceDoubletVector

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)










Inherited by the following classes: [muda::DeviceBCOOVector](classmuda_1_1_device_b_c_o_o_vector.md),  [muda::DeviceBCOOVector](classmuda_1_1_device_b_c_o_o_vector.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; N==1, T, Eigen::Vector&lt; T, N &gt; &gt; | [**ValueT**](#typedef-valuet)  <br> |






## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**IsSegmentVector**](#variable-issegmentvector)   = = (N &gt; 1)<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceDoubletVector**](#function-devicedoubletvector) () = default<br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**count**](#function-count) () const<br> |
|  auto | [**cview**](#function-cview) () const<br> |
|  auto | [**cviewer**](#function-cviewer) () const<br> |
|  auto | [**doublet\_capacity**](#function-doublet_capacity) () const<br> |
|  auto | [**doublet\_count**](#function-doublet_count) () const<br> |
|  auto | [**indices**](#function-indices-12) () <br> |
|  auto | [**indices**](#function-indices-22) () const<br> |
|  void | [**reserve\_doublets**](#function-reserve_doublets) (size\_t nonzero\_count) <br> |
|  void | [**reshape**](#function-reshape) (int num\_segment) <br> |
|  void | [**resize**](#function-resize) (int num\_segment, size\_t nonzero\_count) <br> |
|  void | [**resize\_doublets**](#function-resize_doublets) (size\_t nonzero\_count) <br> |
|  auto | [**values**](#function-values-12) () <br> |
|  auto | [**values**](#function-values-22) () const<br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|  auto | [**viewer**](#function-viewer-12) () <br> |
|  auto | [**viewer**](#function-viewer-22) () const<br> |
|   | [**~DeviceDoubletVector**](#function-devicedoubletvector) () = default<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_count**](#variable-m_count)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_indices**](#variable-m_indices)  <br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; ValueT &gt; | [**m\_values**](#variable-m_values)  <br> |




















## Public Types Documentation




### typedef ValueT 

```C++
using muda::DeviceDoubletVector< T, N >::ValueT =  std::conditional_t<N == 1, T, Eigen::Vector<T, N>>;
```




<hr>
## Public Static Attributes Documentation




### variable IsSegmentVector 

```C++
bool muda::DeviceDoubletVector< T, N >::IsSegmentVector;
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



### function count 

```C++
inline auto muda::DeviceDoubletVector::count () const
```




<hr>



### function cview 

```C++
inline auto muda::DeviceDoubletVector::cview () const
```




<hr>



### function cviewer 

```C++
inline auto muda::DeviceDoubletVector::cviewer () const
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



### function indices [1/2]

```C++
inline auto muda::DeviceDoubletVector::indices () 
```




<hr>



### function indices [2/2]

```C++
inline auto muda::DeviceDoubletVector::indices () const
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



### function values [1/2]

```C++
inline auto muda::DeviceDoubletVector::values () 
```




<hr>



### function values [2/2]

```C++
inline auto muda::DeviceDoubletVector::values () const
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




### variable m\_count 

```C++
int muda::DeviceDoubletVector< T, N >::m_count;
```




<hr>



### variable m\_indices 

```C++
muda::DeviceBuffer<int> muda::DeviceDoubletVector< T, N >::m_indices;
```




<hr>



### variable m\_values 

```C++
muda::DeviceBuffer<ValueT> muda::DeviceDoubletVector< T, N >::m_values;
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

