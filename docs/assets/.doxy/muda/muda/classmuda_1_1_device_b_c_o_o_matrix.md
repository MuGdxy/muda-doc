

# Class muda::DeviceBCOOMatrix

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md)








Inherits the following classes: [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; T, N, N &gt; | [**BlockMatrix**](#typedef-blockmatrix)  <br> |


## Public Types inherited from muda::DeviceTripletMatrix

See [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; T, N, N &gt; | [**BlockMatrix**](classmuda_1_1_device_triplet_matrix.md#typedef-blockmatrix)  <br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBCOOMatrix**](#function-devicebcoomatrix-13) () = default<br> |
|   | [**DeviceBCOOMatrix**](#function-devicebcoomatrix-23) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) &) = default<br> |
|   | [**DeviceBCOOMatrix**](#function-devicebcoomatrix-33) ([**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) &&) = default<br> |
|  auto | [**non\_zero\_blocks**](#function-non_zero_blocks) () const<br> |
|  [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) &) = default<br> |
|  [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) &&) = default<br> |
|   | [**~DeviceBCOOMatrix**](#function-devicebcoomatrix) () = default<br> |


## Public Functions inherited from muda::DeviceTripletMatrix

See [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)

| Type | Name |
| ---: | :--- |
|   | [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md#function-devicetripletmatrix-13) () = default<br> |
|   | [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md#function-devicetripletmatrix-23) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &) = default<br> |
|   | [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md#function-devicetripletmatrix-33) ([**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &&) = default<br> |
|  auto | [**block\_col\_indices**](classmuda_1_1_device_triplet_matrix.md#function-block_col_indices-12) () <br> |
|  auto | [**block\_col\_indices**](classmuda_1_1_device_triplet_matrix.md#function-block_col_indices-22) () const<br> |
|  auto | [**block\_cols**](classmuda_1_1_device_triplet_matrix.md#function-block_cols) () const<br> |
|  auto | [**block\_row\_indices**](classmuda_1_1_device_triplet_matrix.md#function-block_row_indices-12) () <br> |
|  auto | [**block\_row\_indices**](classmuda_1_1_device_triplet_matrix.md#function-block_row_indices-22) () const<br> |
|  auto | [**block\_rows**](classmuda_1_1_device_triplet_matrix.md#function-block_rows) () const<br> |
|  auto | [**block\_values**](classmuda_1_1_device_triplet_matrix.md#function-block_values-12) () <br> |
|  auto | [**block\_values**](classmuda_1_1_device_triplet_matrix.md#function-block_values-22) () const<br> |
|  void | [**clear**](classmuda_1_1_device_triplet_matrix.md#function-clear) () <br> |
|  auto | [**cview**](classmuda_1_1_device_triplet_matrix.md#function-cview) () const<br> |
|  auto | [**cviewer**](classmuda_1_1_device_triplet_matrix.md#function-cviewer) () const<br> |
|   | [**operator CTripletMatrixView&lt; T, N &gt;**](classmuda_1_1_device_triplet_matrix.md#function-operator-ctripletmatrixview<-t,-n->) () const<br> |
|   | [**operator TripletMatrixView&lt; T, N &gt;**](classmuda_1_1_device_triplet_matrix.md#function-operator-tripletmatrixview<-t,-n->) () <br> |
|  [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) & | [**operator=**](classmuda_1_1_device_triplet_matrix.md#function-operator) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &) = default<br> |
|  [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) & | [**operator=**](classmuda_1_1_device_triplet_matrix.md#function-operator_1) ([**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &&) = default<br> |
|  void | [**reserve\_triplets**](classmuda_1_1_device_triplet_matrix.md#function-reserve_triplets) (size\_t nonzero\_count) <br> |
|  void | [**reshape**](classmuda_1_1_device_triplet_matrix.md#function-reshape) (int row, int col) <br> |
|  void | [**resize**](classmuda_1_1_device_triplet_matrix.md#function-resize) (int row, int col, size\_t nonzero\_count) <br> |
|  void | [**resize\_triplets**](classmuda_1_1_device_triplet_matrix.md#function-resize_triplets) (size\_t nonzero\_count) <br> |
|  auto | [**triplet\_capacity**](classmuda_1_1_device_triplet_matrix.md#function-triplet_capacity) () const<br> |
|  auto | [**triplet\_count**](classmuda_1_1_device_triplet_matrix.md#function-triplet_count) () const<br> |
|  auto | [**view**](classmuda_1_1_device_triplet_matrix.md#function-view-12) () <br> |
|  auto | [**view**](classmuda_1_1_device_triplet_matrix.md#function-view-22) () const<br> |
|  auto | [**viewer**](classmuda_1_1_device_triplet_matrix.md#function-viewer) () <br> |
|   | [**~DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md#function-devicetripletmatrix) () = default<br> |




## Public Static Functions inherited from muda::DeviceTripletMatrix

See [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)

| Type | Name |
| ---: | :--- |
|  constexpr int | [**block\_dim**](classmuda_1_1_device_triplet_matrix.md#function-block_dim) () <br> |












## Protected Attributes inherited from muda::DeviceTripletMatrix

See [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)

| Type | Name |
| ---: | :--- |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_col\_indices**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_col_indices)  <br> |
|  int | [**m\_block\_cols**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_cols)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_row\_indices**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_row_indices)  <br> |
|  int | [**m\_block\_rows**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_rows)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; BlockMatrix &gt; | [**m\_block\_values**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_values)  <br> |






































## Public Types Documentation




### typedef BlockMatrix 

```C++
using muda::DeviceBCOOMatrix< T, N >::BlockMatrix =  Eigen::Matrix<T, N, N>;
```




<hr>
## Public Functions Documentation




### function DeviceBCOOMatrix [1/3]

```C++
muda::DeviceBCOOMatrix::DeviceBCOOMatrix () = default
```




<hr>



### function DeviceBCOOMatrix [2/3]

```C++
muda::DeviceBCOOMatrix::DeviceBCOOMatrix (
    const DeviceBCOOMatrix &
) = default
```




<hr>



### function DeviceBCOOMatrix [3/3]

```C++
muda::DeviceBCOOMatrix::DeviceBCOOMatrix (
    DeviceBCOOMatrix &&
) = default
```




<hr>



### function non\_zero\_blocks 

```C++
inline auto muda::DeviceBCOOMatrix::non_zero_blocks () const
```




<hr>



### function operator= 

```C++
DeviceBCOOMatrix & muda::DeviceBCOOMatrix::operator= (
    const DeviceBCOOMatrix &
) = default
```




<hr>



### function operator= 

```C++
DeviceBCOOMatrix & muda::DeviceBCOOMatrix::operator= (
    DeviceBCOOMatrix &&
) = default
```




<hr>



### function ~DeviceBCOOMatrix 

```C++
muda::DeviceBCOOMatrix::~DeviceBCOOMatrix () = default
```




<hr>## Friends Documentation





### friend MatrixFormatConverter&lt; T, N &gt; 

```C++
class muda::DeviceBCOOMatrix::MatrixFormatConverter< T, N > (
    details::MatrixFormatConverter < T, N >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_bcoo_matrix.h`

