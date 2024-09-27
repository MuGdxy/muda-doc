

# Class muda::DeviceTripletMatrix

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)










Inherited by the following classes: [muda::DeviceBCOOMatrix](classmuda_1_1_device_b_c_o_o_matrix.md),  [muda::DeviceBCOOMatrix](classmuda_1_1_device_b_c_o_o_matrix.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; T, N, N &gt; | [**BlockMatrix**](#typedef-blockmatrix)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceTripletMatrix**](#function-devicetripletmatrix-13) () = default<br> |
|   | [**DeviceTripletMatrix**](#function-devicetripletmatrix-23) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &) = default<br> |
|   | [**DeviceTripletMatrix**](#function-devicetripletmatrix-33) ([**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &&) = default<br> |
|  auto | [**block\_col\_indices**](#function-block_col_indices-12) () <br> |
|  auto | [**block\_col\_indices**](#function-block_col_indices-22) () const<br> |
|  auto | [**block\_cols**](#function-block_cols) () const<br> |
|  auto | [**block\_row\_indices**](#function-block_row_indices-12) () <br> |
|  auto | [**block\_row\_indices**](#function-block_row_indices-22) () const<br> |
|  auto | [**block\_rows**](#function-block_rows) () const<br> |
|  auto | [**block\_values**](#function-block_values-12) () <br> |
|  auto | [**block\_values**](#function-block_values-22) () const<br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**cview**](#function-cview) () const<br> |
|  auto | [**cviewer**](#function-cviewer) () const<br> |
|   | [**operator CTripletMatrixView&lt; T, N &gt;**](#function-operator-ctripletmatrixview<-t,-n->) () const<br> |
|   | [**operator TripletMatrixView&lt; T, N &gt;**](#function-operator-tripletmatrixview<-t,-n->) () <br> |
|  [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &) = default<br> |
|  [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &&) = default<br> |
|  void | [**reserve\_triplets**](#function-reserve_triplets) (size\_t nonzero\_count) <br> |
|  void | [**reshape**](#function-reshape) (int row, int col) <br> |
|  void | [**resize**](#function-resize) (int row, int col, size\_t nonzero\_count) <br> |
|  void | [**resize\_triplets**](#function-resize_triplets) (size\_t nonzero\_count) <br> |
|  auto | [**triplet\_capacity**](#function-triplet_capacity) () const<br> |
|  auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|  auto | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceTripletMatrix**](#function-devicetripletmatrix) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  constexpr int | [**block\_dim**](#function-block_dim) () <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_col\_indices**](#variable-m_block_col_indices)  <br> |
|  int | [**m\_block\_cols**](#variable-m_block_cols)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_row\_indices**](#variable-m_block_row_indices)  <br> |
|  int | [**m\_block\_rows**](#variable-m_block_rows)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; BlockMatrix &gt; | [**m\_block\_values**](#variable-m_block_values)  <br> |




















## Public Types Documentation




### typedef BlockMatrix 

```C++
using muda::DeviceTripletMatrix< T, N >::BlockMatrix =  Eigen::Matrix<T, N, N>;
```




<hr>
## Public Functions Documentation




### function DeviceTripletMatrix [1/3]

```C++
muda::DeviceTripletMatrix::DeviceTripletMatrix () = default
```




<hr>



### function DeviceTripletMatrix [2/3]

```C++
muda::DeviceTripletMatrix::DeviceTripletMatrix (
    const DeviceTripletMatrix &
) = default
```




<hr>



### function DeviceTripletMatrix [3/3]

```C++
muda::DeviceTripletMatrix::DeviceTripletMatrix (
    DeviceTripletMatrix &&
) = default
```




<hr>



### function block\_col\_indices [1/2]

```C++
inline auto muda::DeviceTripletMatrix::block_col_indices () 
```




<hr>



### function block\_col\_indices [2/2]

```C++
inline auto muda::DeviceTripletMatrix::block_col_indices () const
```




<hr>



### function block\_cols 

```C++
inline auto muda::DeviceTripletMatrix::block_cols () const
```




<hr>



### function block\_row\_indices [1/2]

```C++
inline auto muda::DeviceTripletMatrix::block_row_indices () 
```




<hr>



### function block\_row\_indices [2/2]

```C++
inline auto muda::DeviceTripletMatrix::block_row_indices () const
```




<hr>



### function block\_rows 

```C++
inline auto muda::DeviceTripletMatrix::block_rows () const
```




<hr>



### function block\_values [1/2]

```C++
inline auto muda::DeviceTripletMatrix::block_values () 
```




<hr>



### function block\_values [2/2]

```C++
inline auto muda::DeviceTripletMatrix::block_values () const
```




<hr>



### function clear 

```C++
inline void muda::DeviceTripletMatrix::clear () 
```




<hr>



### function cview 

```C++
inline auto muda::DeviceTripletMatrix::cview () const
```




<hr>



### function cviewer 

```C++
inline auto muda::DeviceTripletMatrix::cviewer () const
```




<hr>



### function operator CTripletMatrixView&lt; T, N &gt; 

```C++
inline muda::DeviceTripletMatrix::operator CTripletMatrixView< T, N > () const
```




<hr>



### function operator TripletMatrixView&lt; T, N &gt; 

```C++
inline muda::DeviceTripletMatrix::operator TripletMatrixView< T, N > () 
```




<hr>



### function operator= 

```C++
DeviceTripletMatrix & muda::DeviceTripletMatrix::operator= (
    const DeviceTripletMatrix &
) = default
```




<hr>



### function operator= 

```C++
DeviceTripletMatrix & muda::DeviceTripletMatrix::operator= (
    DeviceTripletMatrix &&
) = default
```




<hr>



### function reserve\_triplets 

```C++
inline void muda::DeviceTripletMatrix::reserve_triplets (
    size_t nonzero_count
) 
```




<hr>



### function reshape 

```C++
inline void muda::DeviceTripletMatrix::reshape (
    int row,
    int col
) 
```




<hr>



### function resize 

```C++
inline void muda::DeviceTripletMatrix::resize (
    int row,
    int col,
    size_t nonzero_count
) 
```




<hr>



### function resize\_triplets 

```C++
inline void muda::DeviceTripletMatrix::resize_triplets (
    size_t nonzero_count
) 
```




<hr>



### function triplet\_capacity 

```C++
inline auto muda::DeviceTripletMatrix::triplet_capacity () const
```




<hr>



### function triplet\_count 

```C++
inline auto muda::DeviceTripletMatrix::triplet_count () const
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceTripletMatrix::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceTripletMatrix::view () const
```




<hr>



### function viewer 

```C++
inline auto muda::DeviceTripletMatrix::viewer () 
```




<hr>



### function ~DeviceTripletMatrix 

```C++
muda::DeviceTripletMatrix::~DeviceTripletMatrix () = default
```




<hr>
## Public Static Functions Documentation




### function block\_dim 

```C++
static inline constexpr int muda::DeviceTripletMatrix::block_dim () 
```




<hr>
## Protected Attributes Documentation




### variable m\_block\_col\_indices 

```C++
DeviceBuffer<int> muda::DeviceTripletMatrix< T, N >::m_block_col_indices;
```




<hr>



### variable m\_block\_cols 

```C++
int muda::DeviceTripletMatrix< T, N >::m_block_cols;
```




<hr>



### variable m\_block\_row\_indices 

```C++
DeviceBuffer<int> muda::DeviceTripletMatrix< T, N >::m_block_row_indices;
```




<hr>



### variable m\_block\_rows 

```C++
int muda::DeviceTripletMatrix< T, N >::m_block_rows;
```




<hr>



### variable m\_block\_values 

```C++
DeviceBuffer<BlockMatrix> muda::DeviceTripletMatrix< T, N >::m_block_values;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename U, int M>
class muda::DeviceTripletMatrix::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_triplet_matrix.h`

