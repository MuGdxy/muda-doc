

# Class muda::LinearSystemContext



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**LinearSystemContext**](classmuda_1_1_linear_system_context.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**LinearSystemContext**](#function-linearsystemcontext-13) (const [**LinearSystemContextCreateInfo**](classmuda_1_1_linear_system_context_create_info.md) & info={}) <br> |
|   | [**LinearSystemContext**](#function-linearsystemcontext-23) (const [**LinearSystemContext**](classmuda_1_1_linear_system_context.md) &) = delete<br> |
|   | [**LinearSystemContext**](#function-linearsystemcontext-33) ([**LinearSystemContext**](classmuda_1_1_linear_system_context.md) &&) = delete<br> |
|  void | [**axpby**](#function-axpby-12) (const T & alpha, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, const T & beta, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**axpby**](#function-axpby-22) ([**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; alpha, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; beta, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
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
|  T | [**dot**](#function-dot-13) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**dot**](#function-dot-23) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; result) <br> |
|  void | [**dot**](#function-dot-33) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y, T \* result) <br> |
|  void | [**label**](#function-label-12) (std::string\_view label) <br> |
|  auto | [**label**](#function-label-22) () const<br> |
|  void | [**mv**](#function-mv-13) ([**CDenseMatrixView**](classmuda_1_1_c_dense_matrix_view.md)&lt; T &gt; A, const T & alpha, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, const T & beta, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**mv**](#function-mv-23) ([**CDenseMatrixView**](classmuda_1_1_c_dense_matrix_view.md)&lt; T &gt; A, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; alpha, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; beta, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**mv**](#function-mv-33) ([**CDenseMatrixView**](classmuda_1_1_c_dense_matrix_view.md)&lt; T &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  T | [**norm**](#function-norm-13) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x) <br> |
|  void | [**norm**](#function-norm-23) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; result) <br> |
|  void | [**norm**](#function-norm-33) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, T \* result) <br> |
|  [**LinearSystemContext**](classmuda_1_1_linear_system_context.md) & | [**operator=**](#function-operator) (const [**LinearSystemContext**](classmuda_1_1_linear_system_context.md) &) = delete<br> |
|  [**LinearSystemContext**](classmuda_1_1_linear_system_context.md) & | [**operator=**](#function-operator_1) ([**LinearSystemContext**](classmuda_1_1_linear_system_context.md) &&) = delete<br> |
|  void | [**plus**](#function-plus) ([**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; z) <br> |
|  auto & | [**reorder**](#function-reorder) () <br> |
|  auto | [**reserve\_ratio**](#function-reserve_ratio-12) () const<br> |
|  void | [**reserve\_ratio**](#function-reserve_ratio-22) (float ratio) <br> |
|  void | [**solve**](#function-solve-12) ([**DenseMatrixView**](classmuda_1_1_dense_matrix_view.md)&lt; T &gt; A\_to\_fact, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; b\_to\_x) <br> |
|  void | [**solve**](#function-solve-22) ([**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**CCSRMatrixView**](classmuda_1_1_c_s_r_matrix_view_base.md)&lt; T &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; b) <br> |
|  void | [**spmv**](#function-spmv-18) (const T & a, [**CBSRMatrixView**](classmuda_1_1_b_s_r_matrix_view_base.md)&lt; T, N &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, const T & b, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; & y) <br> |
|  void | [**spmv**](#function-spmv-28) ([**CBSRMatrixView**](classmuda_1_1_b_s_r_matrix_view_base.md)&lt; T, N &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**spmv**](#function-spmv-38) (const T & a, [**CCSRMatrixView**](classmuda_1_1_c_s_r_matrix_view_base.md)&lt; T &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, const T & b, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; & y) <br> |
|  void | [**spmv**](#function-spmv-48) ([**CCSRMatrixView**](classmuda_1_1_c_s_r_matrix_view_base.md)&lt; T &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**spmv**](#function-spmv-58) (const T & a, [**CTripletMatrixView**](classmuda_1_1_triplet_matrix_view_base.md)&lt; T, N &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, const T & b, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; & y) <br> |
|  void | [**spmv**](#function-spmv-68) ([**CTripletMatrixView**](classmuda_1_1_triplet_matrix_view_base.md)&lt; T, N &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  void | [**spmv**](#function-spmv-78) (const T & a, [**CCOOMatrixView**](classmuda_1_1_c_o_o_matrix_view_base.md)&lt; T &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, const T & b, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; & y) <br> |
|  void | [**spmv**](#function-spmv-88) ([**CCOOMatrixView**](classmuda_1_1_c_o_o_matrix_view_base.md)&lt; T &gt; A, [**CDenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; x, [**DenseVectorView**](classmuda_1_1_dense_vector_view_base.md)&lt; T &gt; y) <br> |
|  auto | [**stream**](#function-stream-12) () const<br> |
|  void | [**stream**](#function-stream-22) (cudaStream\_t stream) <br> |
|  void | [**sync**](#function-sync) () <br> |
|  auto & | [**tolerance**](#function-tolerance) () <br> |
|   | [**~LinearSystemContext**](#function-linearsystemcontext) () <br> |




























## Public Functions Documentation




### function LinearSystemContext [1/3]

```C++
muda::LinearSystemContext::LinearSystemContext (
    const LinearSystemContextCreateInfo & info={}
) 
```




<hr>



### function LinearSystemContext [2/3]

```C++
muda::LinearSystemContext::LinearSystemContext (
    const LinearSystemContext &
) = delete
```




<hr>



### function LinearSystemContext [3/3]

```C++
muda::LinearSystemContext::LinearSystemContext (
    LinearSystemContext &&
) = delete
```




<hr>



### function axpby [1/2]

```C++
template<typename T>
void muda::LinearSystemContext::axpby (
    const T & alpha,
    CDenseVectorView < T > x,
    const T & beta,
    DenseVectorView < T > y
) 
```




<hr>



### function axpby [2/2]

```C++
template<typename T>
void muda::LinearSystemContext::axpby (
    CVarView < T > alpha,
    CDenseVectorView < T > x,
    CVarView < T > beta,
    DenseVectorView < T > y
) 
```




<hr>



### function convert [1/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceTripletMatrix < T, N > & from,
    DeviceBCOOMatrix < T, N > & to
) 
```




<hr>



### function convert [2/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceDenseMatrix < T > & to,
    bool clear_dense_matrix=true
) 
```




<hr>



### function convert [3/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function convert [4/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceBCOOMatrix < T, N > & from,
    DeviceBSRMatrix < T, N > & to
) 
```




<hr>



### function convert [5/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceDoubletVector < T, N > & from,
    DeviceBCOOVector < T, N > & to
) 
```




<hr>



### function convert [6/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceBCOOVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [7/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceDoubletVector < T, N > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [8/15]

```C++
template<typename T, int N>
void muda::LinearSystemContext::convert (
    const DeviceBSRMatrix < T, N > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [9/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    const DeviceTripletMatrix < T, 1 > & from,
    DeviceCOOMatrix < T > & to
) 
```




<hr>



### function convert [10/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    const DeviceCOOMatrix < T > & from,
    DeviceDenseMatrix < T > & to,
    bool clear_dense_matrix=true
) 
```




<hr>



### function convert [11/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    const DeviceCOOMatrix < T > & from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [12/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    DeviceCOOMatrix < T > && from,
    DeviceCSRMatrix < T > & to
) 
```




<hr>



### function convert [13/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceCOOVector < T > & to
) 
```




<hr>



### function convert [14/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    const DeviceCOOVector < T > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function convert [15/15]

```C++
template<typename T>
void muda::LinearSystemContext::convert (
    const DeviceDoubletVector < T, 1 > & from,
    DeviceDenseVector < T > & to,
    bool clear_dense_vector=true
) 
```




<hr>



### function dot [1/3]

```C++
template<typename T>
T muda::LinearSystemContext::dot (
    CDenseVectorView < T > x,
    CDenseVectorView < T > y
) 
```




<hr>



### function dot [2/3]

```C++
template<typename T>
void muda::LinearSystemContext::dot (
    CDenseVectorView < T > x,
    CDenseVectorView < T > y,
    VarView < T > result
) 
```




<hr>



### function dot [3/3]

```C++
template<typename T>
void muda::LinearSystemContext::dot (
    CDenseVectorView < T > x,
    CDenseVectorView < T > y,
    T * result
) 
```




<hr>



### function label [1/2]

```C++
inline void muda::LinearSystemContext::label (
    std::string_view label
) 
```




<hr>



### function label [2/2]

```C++
inline auto muda::LinearSystemContext::label () const
```




<hr>



### function mv [1/3]

```C++
template<typename T>
void muda::LinearSystemContext::mv (
    CDenseMatrixView < T > A,
    const T & alpha,
    CDenseVectorView < T > x,
    const T & beta,
    DenseVectorView < T > y
) 
```




<hr>



### function mv [2/3]

```C++
template<typename T>
void muda::LinearSystemContext::mv (
    CDenseMatrixView < T > A,
    CVarView < T > alpha,
    CDenseVectorView < T > x,
    CVarView < T > beta,
    DenseVectorView < T > y
) 
```




<hr>



### function mv [3/3]

```C++
template<typename T>
void muda::LinearSystemContext::mv (
    CDenseMatrixView < T > A,
    CDenseVectorView < T > x,
    DenseVectorView < T > y
) 
```




<hr>



### function norm [1/3]

```C++
template<typename T>
T muda::LinearSystemContext::norm (
    CDenseVectorView < T > x
) 
```




<hr>



### function norm [2/3]

```C++
template<typename T>
void muda::LinearSystemContext::norm (
    CDenseVectorView < T > x,
    VarView < T > result
) 
```




<hr>



### function norm [3/3]

```C++
template<typename T>
void muda::LinearSystemContext::norm (
    CDenseVectorView < T > x,
    T * result
) 
```




<hr>



### function operator= 

```C++
LinearSystemContext & muda::LinearSystemContext::operator= (
    const LinearSystemContext &
) = delete
```




<hr>



### function operator= 

```C++
LinearSystemContext & muda::LinearSystemContext::operator= (
    LinearSystemContext &&
) = delete
```




<hr>



### function plus 

```C++
template<typename T>
void muda::LinearSystemContext::plus (
    CDenseVectorView < T > x,
    CDenseVectorView < T > y,
    DenseVectorView < T > z
) 
```




<hr>



### function reorder 

```C++
inline auto & muda::LinearSystemContext::reorder () 
```




<hr>



### function reserve\_ratio [1/2]

```C++
inline auto muda::LinearSystemContext::reserve_ratio () const
```




<hr>



### function reserve\_ratio [2/2]

```C++
inline void muda::LinearSystemContext::reserve_ratio (
    float ratio
) 
```




<hr>



### function solve [1/2]

```C++
template<typename T>
void muda::LinearSystemContext::solve (
    DenseMatrixView < T > A_to_fact,
    DenseVectorView < T > b_to_x
) 
```




<hr>



### function solve [2/2]

```C++
template<typename T>
void muda::LinearSystemContext::solve (
    DenseVectorView < T > x,
    CCSRMatrixView < T > A,
    CDenseVectorView < T > b
) 
```




<hr>



### function spmv [1/8]

```C++
template<typename T, int N>
void muda::LinearSystemContext::spmv (
    const T & a,
    CBSRMatrixView < T, N > A,
    CDenseVectorView < T > x,
    const T & b,
    DenseVectorView < T > & y
) 
```




<hr>



### function spmv [2/8]

```C++
template<typename T, int N>
void muda::LinearSystemContext::spmv (
    CBSRMatrixView < T, N > A,
    CDenseVectorView < T > x,
    DenseVectorView < T > y
) 
```




<hr>



### function spmv [3/8]

```C++
template<typename T>
void muda::LinearSystemContext::spmv (
    const T & a,
    CCSRMatrixView < T > A,
    CDenseVectorView < T > x,
    const T & b,
    DenseVectorView < T > & y
) 
```




<hr>



### function spmv [4/8]

```C++
template<typename T>
void muda::LinearSystemContext::spmv (
    CCSRMatrixView < T > A,
    CDenseVectorView < T > x,
    DenseVectorView < T > y
) 
```




<hr>



### function spmv [5/8]

```C++
template<typename T, int N>
void muda::LinearSystemContext::spmv (
    const T & a,
    CTripletMatrixView < T, N > A,
    CDenseVectorView < T > x,
    const T & b,
    DenseVectorView < T > & y
) 
```




<hr>



### function spmv [6/8]

```C++
template<typename T, int N>
void muda::LinearSystemContext::spmv (
    CTripletMatrixView < T, N > A,
    CDenseVectorView < T > x,
    DenseVectorView < T > y
) 
```




<hr>



### function spmv [7/8]

```C++
template<typename T>
void muda::LinearSystemContext::spmv (
    const T & a,
    CCOOMatrixView < T > A,
    CDenseVectorView < T > x,
    const T & b,
    DenseVectorView < T > & y
) 
```




<hr>



### function spmv [8/8]

```C++
template<typename T>
void muda::LinearSystemContext::spmv (
    CCOOMatrixView < T > A,
    CDenseVectorView < T > x,
    DenseVectorView < T > y
) 
```




<hr>



### function stream [1/2]

```C++
inline auto muda::LinearSystemContext::stream () const
```




<hr>



### function stream [2/2]

```C++
void muda::LinearSystemContext::stream (
    cudaStream_t stream
) 
```




<hr>



### function sync 

```C++
void muda::LinearSystemContext::sync () 
```




<hr>



### function tolerance 

```C++
inline auto & muda::LinearSystemContext::tolerance () 
```




<hr>



### function ~LinearSystemContext 

```C++
muda::LinearSystemContext::~LinearSystemContext () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/linear_system_context.h`

