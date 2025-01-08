

# Class muda::details::MatrixFormatConverter

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**MatrixFormatConverter**](classmuda_1_1details_1_1_matrix_format_converter.md)








Inherits the following classes: [muda::details::MatrixFormatConverterBase](classmuda_1_1details_1_1_matrix_format_converter_base.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MatrixFormatConverter**](#function-matrixformatconverter) ([**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & handles) <br> |
|  void | [**bsr2csr**](#function-bsr2csr) (cusparseHandle\_t handle, int mb, int nb, int blockDim, cusparseMatDescr\_t descrA, const T \* bsrValA, const int \* bsrRowPtrA, const int \* bsrColIndA, int nnzb, [**DeviceCSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T &gt; & to, [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; & row\_offsets, [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; & col\_indices, [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & values) <br> |
|  void | [**calculate\_block\_offsets**](#function-calculate_block_offsets) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-19) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-29) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md)&lt; T &gt; & to, bool clear\_dense\_matrix=true) <br> |
|  void | [**convert**](#function-convert-39) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-49) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-59) ([**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; && from, [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-69) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-79) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**convert**](#function-convert-89) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**convert**](#function-convert-99) (const [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T, N &gt; & from, [**DeviceCSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**expand\_blocks**](#function-expand_blocks) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**make\_unique\_blocks**](#function-make_unique_blocks) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**make\_unique\_indices**](#function-make_unique_indices-12) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**make\_unique\_indices**](#function-make_unique_indices-22) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & to) <br> |
|  void | [**make\_unique\_indices\_and\_blocks**](#function-make_unique_indices_and_blocks) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**make\_unique\_segments**](#function-make_unique_segments) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & to) <br> |
|  void | [**merge\_sort\_indices\_and\_blocks**](#function-merge_sort_indices_and_blocks) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**merge\_sort\_indices\_and\_segments**](#function-merge_sort_indices_and_segments) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & to) <br> |
|  void | [**radix\_sort\_indices\_and\_blocks**](#function-radix_sort_indices_and_blocks) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**set\_unique\_values\_to\_dense\_vector**](#function-set_unique_values_to_dense_vector) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector) <br> |
|  void | [**sort\_indices\_and\_values**](#function-sort_indices_and_values) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
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
inline muda::details::MatrixFormatConverter::MatrixFormatConverter (
    LinearSystemHandles & handles
) 
```




<hr>



### function bsr2csr 

```C++
inline void muda::details::MatrixFormatConverter::bsr2csr (
    cusparseHandle_t handle,
    int mb,
    int nb,
    int blockDim,
    cusparseMatDescr_t descrA,
    const T * bsrValA,
    const int * bsrRowPtrA,
    const int * bsrColIndA,
    int nnzb,
    DeviceCSRMatrix < T > & to,
    muda::DeviceBuffer < int > & row_offsets,
    muda::DeviceBuffer < int > & col_indices,
    muda::DeviceBuffer < T > & values
) 
```




<hr>



### function calculate\_block\_offsets 

```C++
inline void muda::details::MatrixFormatConverter::calculate_block_offsets (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceBSRMatrix < T, N > & to
) 
```




<hr>



### function convert [1/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function convert [2/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceDenseMatrix < T > & to,
    bool clear_dense_matrix=true
) 
```




<hr>



### function convert [3/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function convert [4/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceBSRMatrix < T, N > & to
) 
```




<hr>



### function convert [5/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    DeviceBCOOMatrix < T, N > && from,
    DeviceBSRMatrix < T, N > & to
) 
```




<hr>



### function convert [6/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceDoubletVector < T, N > & from,
    DeviceBCOOVector < T, N > & to
) 
```




<hr>



### function convert [7/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceBCOOVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [8/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceDoubletVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [9/9]

```C++
inline void muda::details::MatrixFormatConverter::convert (
    const DeviceBSRMatrix < T, N > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function expand\_blocks 

```C++
inline void muda::details::MatrixFormatConverter::expand_blocks (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function make\_unique\_blocks 

```C++
inline void muda::details::MatrixFormatConverter::make_unique_blocks (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function make\_unique\_indices [1/2]

```C++
inline void muda::details::MatrixFormatConverter::make_unique_indices (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function make\_unique\_indices [2/2]

```C++
inline void muda::details::MatrixFormatConverter::make_unique_indices (
    const DeviceDoubletVector < T, N > & from,
    DeviceBCOOVector < T, N > & to
) 
```




<hr>



### function make\_unique\_indices\_and\_blocks 

```C++
inline void muda::details::MatrixFormatConverter::make_unique_indices_and_blocks (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function make\_unique\_segments 

```C++
inline void muda::details::MatrixFormatConverter::make_unique_segments (
    const DeviceDoubletVector < T, N > & from,
    DeviceBCOOVector < T, N > & to
) 
```




<hr>



### function merge\_sort\_indices\_and\_blocks 

```C++
inline void muda::details::MatrixFormatConverter::merge_sort_indices_and_blocks (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function merge\_sort\_indices\_and\_segments 

```C++
inline void muda::details::MatrixFormatConverter::merge_sort_indices_and_segments (
    const DeviceDoubletVector < T, N > & from,
    DeviceBCOOVector < T, N > & to
) 
```




<hr>



### function radix\_sort\_indices\_and\_blocks 

```C++
inline void muda::details::MatrixFormatConverter::radix_sort_indices_and_blocks (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function set\_unique\_values\_to\_dense\_vector 

```C++
inline void muda::details::MatrixFormatConverter::set_unique_values_to_dense_vector (
    const DeviceBCOOVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector
) 
```




<hr>



### function sort\_indices\_and\_values 

```C++
inline void muda::details::MatrixFormatConverter::sort_indices_and_values (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function ~MatrixFormatConverter 

```C++
virtual muda::details::MatrixFormatConverter::~MatrixFormatConverter () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_bcoo_matrix.h`

