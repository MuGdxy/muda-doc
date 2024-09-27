

# Class muda::DeviceBCOOVector&lt; T, 1 &gt;

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBCOOVector&lt; T, 1 &gt;**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)








Inherits the following classes: [muda::DeviceDoubletVector&lt; T, 1 &gt;](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBCOOVector**](#function-devicebcoovector-13) () = default<br> |
|   | [**DeviceBCOOVector**](#function-devicebcoovector-23) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) & other) <br> |
|   | [**DeviceBCOOVector**](#function-devicebcoovector-33) ([**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) && other) <br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**non\_zeros**](#function-non_zeros) () const<br> |
|  [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) & | [**operator=**](#function-operator) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) & other) <br> |
|  [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) & | [**operator=**](#function-operator_1) ([**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md) && other) <br> |
|  auto | [**view**](#function-view) () <br> |
|   | [**~DeviceBCOOVector**](#function-devicebcoovector) () <br> |


## Public Functions inherited from muda::DeviceDoubletVector< T, 1 >

See [muda::DeviceDoubletVector&lt; T, 1 &gt;](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md)

| Type | Name |
| ---: | :--- |
|   | [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-devicedoubletvector) () = default<br> |
|  void | [**clear**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-clear) () <br> |
|  auto | [**doublet\_count**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-doublet_count) () const<br> |
|  auto | [**indices**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-indices-12) () <br> |
|  auto | [**indices**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-indices-22) () const<br> |
|  void | [**reshape**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-reshape) (int num) <br> |
|  void | [**resize**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-resize) (int num, size\_t nonzero\_count) <br> |
|  void | [**resize\_doublet**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-resize_doublet) (size\_t nonzero\_count) <br> |
|  auto | [**size**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-size) () const<br> |
|  auto | [**values**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-values-12) () <br> |
|  auto | [**values**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-values-22) () const<br> |
|  auto | [**view**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-view-12) () <br> |
|  auto | [**view**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-view-22) () const<br> |
|  auto | [**viewer**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-viewer-12) () <br> |
|  auto | [**viewer**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-viewer-22) () const<br> |
|   | [**~DeviceDoubletVector**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#function-devicedoubletvector) () = default<br> |














## Protected Attributes

| Type | Name |
| ---: | :--- |
|  cusparseSpVecDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |


## Protected Attributes inherited from muda::DeviceDoubletVector< T, 1 >

See [muda::DeviceDoubletVector&lt; T, 1 &gt;](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md)

| Type | Name |
| ---: | :--- |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_indices**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#variable-m_indices)  <br> |
|  int | [**m\_size**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#variable-m_size)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; | [**m\_values**](classmuda_1_1_device_doublet_vector_3_01_t_00_011_01_4.md#variable-m_values)  <br> |






































## Public Functions Documentation




### function DeviceBCOOVector [1/3]

```C++
muda::DeviceBCOOVector< T, 1 >::DeviceBCOOVector () = default
```




<hr>



### function DeviceBCOOVector [2/3]

```C++
inline muda::DeviceBCOOVector< T, 1 >::DeviceBCOOVector (
    const DeviceBCOOVector & other
) 
```




<hr>



### function DeviceBCOOVector [3/3]

```C++
inline muda::DeviceBCOOVector< T, 1 >::DeviceBCOOVector (
    DeviceBCOOVector && other
) 
```




<hr>



### function descr 

```C++
inline auto muda::DeviceBCOOVector< T, 1 >::descr () const
```




<hr>



### function non\_zeros 

```C++
inline auto muda::DeviceBCOOVector< T, 1 >::non_zeros () const
```




<hr>



### function operator= 

```C++
inline DeviceBCOOVector & muda::DeviceBCOOVector< T, 1 >::operator= (
    const DeviceBCOOVector & other
) 
```




<hr>



### function operator= 

```C++
inline DeviceBCOOVector & muda::DeviceBCOOVector< T, 1 >::operator= (
    DeviceBCOOVector && other
) 
```




<hr>



### function view 

```C++
inline auto muda::DeviceBCOOVector< T, 1 >::view () 
```




<hr>



### function ~DeviceBCOOVector 

```C++
inline muda::DeviceBCOOVector< T, 1 >::~DeviceBCOOVector () 
```




<hr>
## Protected Attributes Documentation




### variable m\_descr 

```C++
cusparseSpVecDescr_t muda::DeviceBCOOVector< T, 1 >::m_descr;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename U, int N>
class muda::DeviceBCOOVector< T, 1 >::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_bcoo_vector.h`

