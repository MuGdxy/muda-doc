

# Class muda::MatrixFormatConverter



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**MatrixFormatConverter**](classmuda_1_1_matrix_format_converter.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MatrixFormatConverter**](#function-matrixformatconverter) ([**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & handles) <br> |
|  void | [**convert**](#function-convert-115) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, N &gt; & from, [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-215) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md)&lt; T &gt; & to, bool clear\_dense\_matrix=true) <br> |
|  void | [**convert**](#function-convert-315) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-415) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T, N &gt; & from, [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-515) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & to) <br> |
|  void | [**convert**](#function-convert-615) (const [**DeviceBCOOVector**](classmuda_1_1_device_b_c_o_o_vector.md)&lt; T, N &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**convert**](#function-convert-715) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, N &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**convert**](#function-convert-815) (const [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)&lt; T, N &gt; & from, [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-915) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)&lt; T, 1 &gt; & from, [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-1015) (const [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & from, [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md)&lt; T &gt; & to, bool clear\_dense\_matrix=true) <br> |
|  void | [**convert**](#function-convert-1115) (const [**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; & from, [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-1215) ([**DeviceCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)&lt; T &gt; && from, [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-1315) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & to) <br> |
|  void | [**convert**](#function-convert-1415) (const [**DeviceCOOVector**](classmuda_1_1_device_b_c_o_o_vector_3_01_t_00_011_01_4.md)&lt; T &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|  void | [**convert**](#function-convert-1515) (const [**DeviceDoubletVector**](classmuda_1_1_device_doublet_vector.md)&lt; T, 1 &gt; & from, [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)&lt; T &gt; & to, bool clear\_dense\_vector=true) <br> |
|   | [**~MatrixFormatConverter**](#function-matrixformatconverter) () <br> |




























## Public Functions Documentation




### function MatrixFormatConverter 

```C++
inline muda::MatrixFormatConverter::MatrixFormatConverter (
    LinearSystemHandles & handles
) 
```




<hr>



### function convert [1/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function convert [2/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceDenseMatrix < T > & to,
    bool clear_dense_matrix=true
) 
```




<hr>



### function convert [3/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function convert [4/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceBSRMatrix < T, N > & to
) 
```




<hr>



### function convert [5/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceDoubletVector < T, N > & from,
    DeviceBCOOVector < T, N > & to
) 
```




<hr>



### function convert [6/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceBCOOVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [7/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceDoubletVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [8/15]

```C++
template<typename T, int N>
void muda::MatrixFormatConverter::convert (
    const DeviceBSRMatrix < T, N > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [9/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function convert [10/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    const DeviceCOOMatrix < T > & from,
    DeviceDenseMatrix < T > & to,
    bool clear_dense_matrix=true
) 
```




<hr>



### function convert [11/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    const DeviceCOOMatrix < T > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [12/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    DeviceCOOMatrix < T > && from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [13/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceCOOVector < T > & to
) 
```




<hr>



### function convert [14/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    const DeviceCOOVector < T > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [15/15]

```C++
template<typename T>
void muda::MatrixFormatConverter::convert (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function ~MatrixFormatConverter 

```C++
muda::MatrixFormatConverter::~MatrixFormatConverter () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/matrix_format_converter.h`

