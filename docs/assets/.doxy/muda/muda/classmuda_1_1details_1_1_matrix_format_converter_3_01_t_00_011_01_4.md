

# Class muda::details::MatrixFormatConverter&lt; T, 1 &gt;

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**MatrixFormatConverter&lt; T, 1 &gt;**](classmuda_1_1details_1_1_matrix_format_converter_3_01_t_00_011_01_4.md)








Inherits the following classes: [muda::details::MatrixFormatConverterBase](classmuda_1_1details_1_1_matrix_format_converter_base.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MatrixFormatConverter**](#function-matrixformatconverter) ([**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & handles) <br> |
|  void | [**calculate\_block\_offsets**](#function-calculate_block_offsets) (const [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & from, [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-17) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-27) (const [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & from, [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md)&lt; T &gt; & to, bool clear\_dense\_matrix=true) <br> |
|  void | [**convert**](#function-convert-37) (const [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & from, [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-47) ([**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; && from, [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-57) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-67) (const [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**convert**](#function-convert-77) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**make\_unique\_indices**](#function-make_unique_indices-12) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**make\_unique\_indices**](#function-make_unique_indices-22) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & to) <br> |
|  void | [**make\_unique\_indices\_and\_blocks**](#function-make_unique_indices_and_blocks) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, 1 &gt; & to) <br> |
|  void | [**make\_unique\_values**](#function-make_unique_values-12) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**make\_unique\_values**](#function-make_unique_values-22) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & to) <br> |
|  void | [**merge\_sort\_indices\_and\_values**](#function-merge_sort_indices_and_values-12) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**merge\_sort\_indices\_and\_values**](#function-merge_sort_indices_and_values-22) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & to) <br> |
|  void | [**radix\_sort\_indices\_and\_blocks**](#function-radix_sort_indices_and_blocks) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, 1 &gt; & to) <br> |
|  void | [**set\_unique\_values\_to\_dense\_vector**](#function-set_unique_values_to_dense_vector) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector) <br> |
| virtual  | [**~MatrixFormatConverter**](#function-matrixformatconverter) () = default<br> |


## Public Functions inherited from muda::details::MatrixFormatConverterBase

See [muda::details::MatrixFormatConverterBase](classmuda_1_1details_1_1_matrix_format_converter_base.md)

| Type | Name |
| ---: | :--- |
|   | [**MatrixFormatConverterBase**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-matrixformatconverterbase) ([**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & context, cudaDataType\_t data\_type, int N) <br> |
|  auto | [**cublas**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-cublas) () const<br> |
|  auto | [**cusolver\_dn**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-cusolver_dn) () const<br> |
|  auto | [**cusolver\_sp**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-cusolver_sp) () const<br> |
|  auto | [**cusparse**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-cusparse) () const<br> |
|  auto | [**data\_type**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-data_type) () const<br> |
|  auto | [**dim**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-dim) () const<br> |
|  void | [**loose\_resize**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-loose_resize) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buf, size\_t new\_size) <br> |
| virtual  | [**~MatrixFormatConverterBase**](classmuda_1_1details_1_1_matrix_format_converter_base.md#function-matrixformatconverterbase) () = default<br> |
















## Protected Attributes inherited from muda::details::MatrixFormatConverterBase

See [muda::details::MatrixFormatConverterBase](classmuda_1_1details_1_1_matrix_format_converter_base.md)

| Type | Name |
| ---: | :--- |
|  int | [**m\_N**](classmuda_1_1details_1_1_matrix_format_converter_base.md#variable-m_n)  <br> |
|  cudaDataType\_t | [**m\_data\_type**](classmuda_1_1details_1_1_matrix_format_converter_base.md#variable-m_data_type)  <br> |
|  [**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & | [**m\_handles**](classmuda_1_1details_1_1_matrix_format_converter_base.md#variable-m_handles)  <br> |






































## Public Functions Documentation




### function MatrixFormatConverter 

```C++
inline muda::details::MatrixFormatConverter< T, 1 >::MatrixFormatConverter (
    LinearSystemHandles & handles
) 
```




<hr>



### function calculate\_block\_offsets 

```C++
void muda::details::MatrixFormatConverter< T, 1 >::calculate_block_offsets (
    const DeviceCOOMatrix < T > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [1/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function convert [2/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    const DeviceCOOMatrix < T > & from,
    DeviceDenseMatrix < T > & to,
    bool clear_dense_matrix=true
) 
```




<hr>



### function convert [3/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    const DeviceCOOMatrix < T > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [4/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    DeviceCOOMatrix < T > && from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [5/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceCOOVector < T > & to
) 
```




<hr>



### function convert [6/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    const DeviceCOOVector < T > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [7/7]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::convert (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function make\_unique\_indices [1/2]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::make_unique_indices (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function make\_unique\_indices [2/2]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::make_unique_indices (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceCOOVector < T > & to
) 
```




<hr>



### function make\_unique\_indices\_and\_blocks 

```C++
void muda::details::MatrixFormatConverter< T, 1 >::make_unique_indices_and_blocks (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceBCOOMatrix < T, 1 > & to
) 
```




<hr>



### function make\_unique\_values [1/2]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::make_unique_values (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function make\_unique\_values [2/2]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::make_unique_values (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceCOOVector < T > & to
) 
```




<hr>



### function merge\_sort\_indices\_and\_values [1/2]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::merge_sort_indices_and_values (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function merge\_sort\_indices\_and\_values [2/2]

```C++
void muda::details::MatrixFormatConverter< T, 1 >::merge_sort_indices_and_values (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceCOOVector < T > & to
) 
```




<hr>



### function radix\_sort\_indices\_and\_blocks 

```C++
void muda::details::MatrixFormatConverter< T, 1 >::radix_sort_indices_and_blocks (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceBCOOMatrix < T, 1 > & to
) 
```




<hr>



### function set\_unique\_values\_to\_dense\_vector 

```C++
void muda::details::MatrixFormatConverter< T, 1 >::set_unique_values_to_dense_vector (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector
) 
```




<hr>



### function ~MatrixFormatConverter 

```C++
virtual muda::details::MatrixFormatConverter< T, 1 >::~MatrixFormatConverter () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/matrix_format_converter_impl.h`

