

# Class muda::DeviceBSRMatrix

**template &lt;typename Ty, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; Ty, N, N &gt; | [**BlockMatrix**](#typedef-blockmatrix)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBSRMatrix**](#function-devicebsrmatrix-13) () = default<br> |
|   | [**DeviceBSRMatrix**](#function-devicebsrmatrix-23) (const [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md) &) <br> |
|   | [**DeviceBSRMatrix**](#function-devicebsrmatrix-33) ([**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md) &&) <br> |
|  auto | [**T**](#function-t-12) () const<br> |
|  auto | [**T**](#function-t-22) () <br> |
|  auto | [**block\_col\_indices**](#function-block_col_indices-12) () <br> |
|  auto | [**block\_col\_indices**](#function-block_col_indices-22) () const<br> |
|  auto | [**block\_cols**](#function-block_cols) () const<br> |
|  auto | [**block\_row\_offsets**](#function-block_row_offsets-12) () <br> |
|  auto | [**block\_row\_offsets**](#function-block_row_offsets-22) () const<br> |
|  auto | [**block\_rows**](#function-block_rows) () const<br> |
|  auto | [**block\_values**](#function-block_values-12) () <br> |
|  auto | [**block\_values**](#function-block_values-22) () const<br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**cview**](#function-cview) () const<br> |
|  cusparseSpMatDescr\_t | [**descr**](#function-descr) () const<br> |
|  cusparseMatDescr\_t | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  auto | [**non\_zero\_blocks**](#function-non_zero_blocks) () const<br> |
|   | [**operator BSRMatrixView&lt; Ty, N &gt;**](#function-operator-bsrmatrixview<-ty,-n->) () <br> |
|   | [**operator CBSRMatrixView&lt; Ty, N &gt;**](#function-operator-cbsrmatrixview<-ty,-n->) () const<br> |
|  [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md) &) <br> |
|  [**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceBSRMatrix**](classmuda_1_1_device_b_s_r_matrix.md) &&) <br> |
|  void | [**reserve**](#function-reserve) (int non\_zero\_blocks) <br> |
|  void | [**reserve\_offsets**](#function-reserve_offsets) (int size) <br> |
|  void | [**reshape**](#function-reshape) (int row, int col) <br> |
|  void | [**resize**](#function-resize) (int non\_zero\_blocks) <br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|   | [**~DeviceBSRMatrix**](#function-devicebsrmatrix) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  constexpr int | [**block\_size**](#function-block_size) () <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_col\_indices**](#variable-m_block_col_indices)  <br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_row\_offsets**](#variable-m_block_row_offsets)  <br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; BlockMatrix &gt; | [**m\_block\_values**](#variable-m_block_values)  <br> |
|  int | [**m\_col**](#variable-m_col)   = = 0<br> |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |
|  int | [**m\_row**](#variable-m_row)   = = 0<br> |




















## Public Types Documentation




### typedef BlockMatrix 

```C++
using muda::DeviceBSRMatrix< Ty, N >::BlockMatrix =  Eigen::Matrix<Ty, N, N>;
```




<hr>
## Public Functions Documentation




### function DeviceBSRMatrix [1/3]

```C++
muda::DeviceBSRMatrix::DeviceBSRMatrix () = default
```




<hr>



### function DeviceBSRMatrix [2/3]

```C++
muda::DeviceBSRMatrix::DeviceBSRMatrix (
    const DeviceBSRMatrix &
) 
```




<hr>



### function DeviceBSRMatrix [3/3]

```C++
muda::DeviceBSRMatrix::DeviceBSRMatrix (
    DeviceBSRMatrix &&
) 
```




<hr>



### function T [1/2]

```C++
inline auto muda::DeviceBSRMatrix::T () const
```




<hr>



### function T [2/2]

```C++
inline auto muda::DeviceBSRMatrix::T () 
```




<hr>



### function block\_col\_indices [1/2]

```C++
inline auto muda::DeviceBSRMatrix::block_col_indices () 
```




<hr>



### function block\_col\_indices [2/2]

```C++
inline auto muda::DeviceBSRMatrix::block_col_indices () const
```




<hr>



### function block\_cols 

```C++
inline auto muda::DeviceBSRMatrix::block_cols () const
```




<hr>



### function block\_row\_offsets [1/2]

```C++
inline auto muda::DeviceBSRMatrix::block_row_offsets () 
```




<hr>



### function block\_row\_offsets [2/2]

```C++
inline auto muda::DeviceBSRMatrix::block_row_offsets () const
```




<hr>



### function block\_rows 

```C++
inline auto muda::DeviceBSRMatrix::block_rows () const
```




<hr>



### function block\_values [1/2]

```C++
inline auto muda::DeviceBSRMatrix::block_values () 
```




<hr>



### function block\_values [2/2]

```C++
inline auto muda::DeviceBSRMatrix::block_values () const
```




<hr>



### function clear 

```C++
void muda::DeviceBSRMatrix::clear () 
```




<hr>



### function cview 

```C++
inline auto muda::DeviceBSRMatrix::cview () const
```




<hr>



### function descr 

```C++
cusparseSpMatDescr_t muda::DeviceBSRMatrix::descr () const
```




<hr>



### function legacy\_descr 

```C++
cusparseMatDescr_t muda::DeviceBSRMatrix::legacy_descr () const
```




<hr>



### function non\_zero\_blocks 

```C++
inline auto muda::DeviceBSRMatrix::non_zero_blocks () const
```




<hr>



### function operator BSRMatrixView&lt; Ty, N &gt; 

```C++
inline muda::DeviceBSRMatrix::operator BSRMatrixView< Ty, N > () 
```




<hr>



### function operator CBSRMatrixView&lt; Ty, N &gt; 

```C++
inline muda::DeviceBSRMatrix::operator CBSRMatrixView< Ty, N > () const
```




<hr>



### function operator= 

```C++
DeviceBSRMatrix & muda::DeviceBSRMatrix::operator= (
    const DeviceBSRMatrix &
) 
```




<hr>



### function operator= 

```C++
DeviceBSRMatrix & muda::DeviceBSRMatrix::operator= (
    DeviceBSRMatrix &&
) 
```




<hr>



### function reserve 

```C++
void muda::DeviceBSRMatrix::reserve (
    int non_zero_blocks
) 
```




<hr>



### function reserve\_offsets 

```C++
void muda::DeviceBSRMatrix::reserve_offsets (
    int size
) 
```




<hr>



### function reshape 

```C++
void muda::DeviceBSRMatrix::reshape (
    int row,
    int col
) 
```




<hr>



### function resize 

```C++
void muda::DeviceBSRMatrix::resize (
    int non_zero_blocks
) 
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceBSRMatrix::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceBSRMatrix::view () const
```




<hr>



### function ~DeviceBSRMatrix 

```C++
muda::DeviceBSRMatrix::~DeviceBSRMatrix () 
```




<hr>
## Public Static Functions Documentation




### function block\_size 

```C++
static inline constexpr int muda::DeviceBSRMatrix::block_size () 
```




<hr>
## Protected Attributes Documentation




### variable m\_block\_col\_indices 

```C++
muda::DeviceBuffer<int> muda::DeviceBSRMatrix< Ty, N >::m_block_col_indices;
```




<hr>



### variable m\_block\_row\_offsets 

```C++
muda::DeviceBuffer<int> muda::DeviceBSRMatrix< Ty, N >::m_block_row_offsets;
```




<hr>



### variable m\_block\_values 

```C++
muda::DeviceBuffer<BlockMatrix> muda::DeviceBSRMatrix< Ty, N >::m_block_values;
```




<hr>



### variable m\_col 

```C++
int muda::DeviceBSRMatrix< Ty, N >::m_col;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::DeviceBSRMatrix< Ty, N >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::DeviceBSRMatrix< Ty, N >::m_legacy_descr;
```




<hr>



### variable m\_row 

```C++
int muda::DeviceBSRMatrix< Ty, N >::m_row;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter&lt; Ty, N &gt; 

```C++
class muda::DeviceBSRMatrix::MatrixFormatConverter< Ty, N > (
    details::MatrixFormatConverter < Ty, N >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_bsr_matrix.h`

