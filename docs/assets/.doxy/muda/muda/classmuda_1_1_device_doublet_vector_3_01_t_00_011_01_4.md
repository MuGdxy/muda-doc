

# Class muda::DeviceDoubletVector&lt; T, 1 &gt;

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceDoubletVector&lt; T, 1 &gt;**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md)










Inherited by the following classes: [muda::DeviceBCOOVector&lt; T, 1 &gt;](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceDoubletVector**](#function-devicedoubletvector) () = default<br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**doublet\_count**](#function-doublet_count) () const<br> |
|  auto | [**indices**](#function-indices-12) () <br> |
|  auto | [**indices**](#function-indices-22) () const<br> |
|  void | [**reshape**](#function-reshape) (int num) <br> |
|  void | [**resize**](#function-resize) (int num, size\_t nonzero\_count) <br> |
|  void | [**resize\_doublet**](#function-resize_doublet) (size\_t nonzero\_count) <br> |
|  auto | [**size**](#function-size) () const<br> |
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
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_indices**](#variable-m_indices)  <br> |
|  int | [**m\_size**](#variable-m_size)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; | [**m\_values**](#variable-m_values)  <br> |




















## Public Functions Documentation




### function DeviceDoubletVector 

```C++
muda::DeviceDoubletVector< T, 1 >::DeviceDoubletVector () = default
```




<hr>



### function clear 

```C++
inline void muda::DeviceDoubletVector< T, 1 >::clear () 
```




<hr>



### function doublet\_count 

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::doublet_count () const
```




<hr>



### function indices [1/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::indices () 
```




<hr>



### function indices [2/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::indices () const
```




<hr>



### function reshape 

```C++
inline void muda::DeviceDoubletVector< T, 1 >::reshape (
    int num
) 
```




<hr>



### function resize 

```C++
inline void muda::DeviceDoubletVector< T, 1 >::resize (
    int num,
    size_t nonzero_count
) 
```




<hr>



### function resize\_doublet 

```C++
inline void muda::DeviceDoubletVector< T, 1 >::resize_doublet (
    size_t nonzero_count
) 
```




<hr>



### function size 

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::size () const
```




<hr>



### function values [1/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::values () 
```




<hr>



### function values [2/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::values () const
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::view () const
```




<hr>



### function viewer [1/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::viewer () 
```




<hr>



### function viewer [2/2]

```C++
inline auto muda::DeviceDoubletVector< T, 1 >::viewer () const
```




<hr>



### function ~DeviceDoubletVector 

```C++
muda::DeviceDoubletVector< T, 1 >::~DeviceDoubletVector () = default
```




<hr>
## Protected Attributes Documentation




### variable m\_indices 

```C++
muda::DeviceBuffer<int> muda::DeviceDoubletVector< T, 1 >::m_indices;
```




<hr>



### variable m\_size 

```C++
int muda::DeviceDoubletVector< T, 1 >::m_size;
```




<hr>



### variable m\_values 

```C++
muda::DeviceBuffer<T> muda::DeviceDoubletVector< T, 1 >::m_values;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename U, int M>
class muda::DeviceDoubletVector< T, 1 >::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_doublet_vector.h`

