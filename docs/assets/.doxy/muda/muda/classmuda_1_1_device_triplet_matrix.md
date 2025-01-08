

# Class muda::DeviceTripletMatrix

**template &lt;typename T, int N&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md)










Inherited by the following classes: [muda::DeviceBCOOMatrix](classmuda_1_1_device_b_c_o_o_matrix.md),  [muda::DeviceBCOOMatrix](classmuda_1_1_device_b_c_o_o_matrix.md),  [muda::DeviceBCOOMatrix](classmuda_1_1_device_b_c_o_o_matrix.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; N==1, T, Eigen::Matrix&lt; T, N, N &gt; &gt; | [**ValueT**](#typedef-valuet)  <br> |






## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**IsBlockMatrix**](#variable-isblockmatrix)   = = (N &gt; 1)<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceTripletMatrix**](#function-devicetripletmatrix-13) () = default<br> |
|   | [**DeviceTripletMatrix**](#function-devicetripletmatrix-23) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &) = default<br> |
|   | [**DeviceTripletMatrix**](#function-devicetripletmatrix-33) ([**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &&) = default<br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**col\_indices**](#function-col_indices-12) () <br> |
|  auto | [**col\_indices**](#function-col_indices-22) () const<br> |
|  auto | [**cols**](#function-cols) () const<br> |
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
|  auto | [**row\_indices**](#function-row_indices-12) () <br> |
|  auto | [**row\_indices**](#function-row_indices-22) () const<br> |
|  auto | [**rows**](#function-rows) () const<br> |
|  auto | [**triplet\_capacity**](#function-triplet_capacity) () const<br> |
|  auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  auto | [**values**](#function-values-12) () <br> |
|  auto | [**values**](#function-values-22) () const<br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|  auto | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceTripletMatrix**](#function-devicetripletmatrix) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  int | [**block\_dim**](#function-block_dim) () <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_col\_indices**](#variable-m_col_indices)  <br> |
|  int | [**m\_cols**](#variable-m_cols)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_row\_indices**](#variable-m_row_indices)  <br> |
|  int | [**m\_rows**](#variable-m_rows)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; ValueT &gt; | [**m\_values**](#variable-m_values)  <br> |




















## Public Types Documentation




### typedef ValueT 

```C++
using muda::DeviceTripletMatrix< T, N >::ValueT =  std::conditional_t<N == 1, T, Eigen::Matrix<T, N, N>>;
```




<hr>
## Public Static Attributes Documentation




### variable IsBlockMatrix 

```C++
bool muda::DeviceTripletMatrix< T, N >::IsBlockMatrix;
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



### function clear 

```C++
inline void muda::DeviceTripletMatrix::clear () 
```




<hr>



### function col\_indices [1/2]

```C++
inline auto muda::DeviceTripletMatrix::col_indices () 
```




<hr>



### function col\_indices [2/2]

```C++
inline auto muda::DeviceTripletMatrix::col_indices () const
```




<hr>



### function cols 

```C++
inline auto muda::DeviceTripletMatrix::cols () const
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



### function row\_indices [1/2]

```C++
inline auto muda::DeviceTripletMatrix::row_indices () 
```




<hr>



### function row\_indices [2/2]

```C++
inline auto muda::DeviceTripletMatrix::row_indices () const
```




<hr>



### function rows 

```C++
inline auto muda::DeviceTripletMatrix::rows () const
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



### function values [1/2]

```C++
inline auto muda::DeviceTripletMatrix::values () 
```




<hr>



### function values [2/2]

```C++
inline auto muda::DeviceTripletMatrix::values () const
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
static inline int muda::DeviceTripletMatrix::block_dim () 
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_indices 

```C++
DeviceBuffer<int> muda::DeviceTripletMatrix< T, N >::m_col_indices;
```




<hr>



### variable m\_cols 

```C++
int muda::DeviceTripletMatrix< T, N >::m_cols;
```




<hr>



### variable m\_row\_indices 

```C++
DeviceBuffer<int> muda::DeviceTripletMatrix< T, N >::m_row_indices;
```




<hr>



### variable m\_rows 

```C++
int muda::DeviceTripletMatrix< T, N >::m_rows;
```




<hr>



### variable m\_values 

```C++
DeviceBuffer<ValueT> muda::DeviceTripletMatrix< T, N >::m_values;
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

