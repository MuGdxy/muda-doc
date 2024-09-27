

# Class muda::DeviceBCOOMatrix&lt; Ty, 1 &gt;

**template &lt;typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceBCOOMatrix&lt; Ty, 1 &gt;**](classmuda_1_1_device_b_c_o_o_matrix_3_01_ty_00_011_01_4.md)








Inherits the following classes: [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)
















## Public Types inherited from muda::DeviceTripletMatrix

See [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)

| Type | Name |
| ---: | :--- |
| typedef Eigen::Matrix&lt; T, N, N &gt; | [**BlockMatrix**](classmuda_1_1_device_triplet_matrix.md#typedef-blockmatrix)  <br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceBCOOMatrix**](#function-devicebcoomatrix-13) () = default<br> |
|   | [**DeviceBCOOMatrix**](#function-devicebcoomatrix-23) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) & other) <br> |
|   | [**DeviceBCOOMatrix**](#function-devicebcoomatrix-33) ([**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) && other) <br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**cview**](#function-cview) () const<br> |
|  auto | [**cviewer**](#function-cviewer) () const<br> |
|  auto | [**descr**](#function-descr) () const<br> |
|  auto | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  auto | [**non\_zeros**](#function-non_zeros) () const<br> |
|   | [**operator CCOOMatrixView&lt; Ty &gt;**](#function-operator-ccoomatrixview<-ty->) () const<br> |
|   | [**operator COOMatrixView&lt; Ty &gt;**](#function-operator-coomatrixview<-ty->) () <br> |
|  [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) & other) <br> |
|  [**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceBCOOMatrix**](classmuda_1_1_device_b_c_o_o_matrix.md) && other) <br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|  auto | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceBCOOMatrix**](#function-devicebcoomatrix) () <br> |


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










## Protected Attributes

| Type | Name |
| ---: | :--- |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |


## Protected Attributes inherited from muda::DeviceTripletMatrix

See [muda::DeviceTripletMatrix](classmuda_1_1_device_triplet_matrix.md)

| Type | Name |
| ---: | :--- |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_col\_indices**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_col_indices)  <br> |
|  int | [**m\_block\_cols**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_cols)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_block\_row\_indices**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_row_indices)  <br> |
|  int | [**m\_block\_rows**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_rows)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; BlockMatrix &gt; | [**m\_block\_values**](classmuda_1_1_device_triplet_matrix.md#variable-m_block_values)  <br> |






































## Public Functions Documentation




### function DeviceBCOOMatrix [1/3]

```C++
muda::DeviceBCOOMatrix< Ty, 1 >::DeviceBCOOMatrix () = default
```




<hr>



### function DeviceBCOOMatrix [2/3]

```C++
inline muda::DeviceBCOOMatrix< Ty, 1 >::DeviceBCOOMatrix (
    const DeviceBCOOMatrix & other
) 
```




<hr>



### function DeviceBCOOMatrix [3/3]

```C++
inline muda::DeviceBCOOMatrix< Ty, 1 >::DeviceBCOOMatrix (
    DeviceBCOOMatrix && other
) 
```




<hr>



### function clear 

```C++
inline void muda::DeviceBCOOMatrix< Ty, 1 >::clear () 
```




<hr>



### function cview 

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::cview () const
```




<hr>



### function cviewer 

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::cviewer () const
```




<hr>



### function descr 

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::descr () const
```




<hr>



### function legacy\_descr 

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::legacy_descr () const
```




<hr>



### function non\_zeros 

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::non_zeros () const
```




<hr>



### function operator CCOOMatrixView&lt; Ty &gt; 

```C++
inline muda::DeviceBCOOMatrix< Ty, 1 >::operator CCOOMatrixView< Ty > () const
```




<hr>



### function operator COOMatrixView&lt; Ty &gt; 

```C++
inline muda::DeviceBCOOMatrix< Ty, 1 >::operator COOMatrixView< Ty > () 
```




<hr>



### function operator= 

```C++
inline DeviceBCOOMatrix & muda::DeviceBCOOMatrix< Ty, 1 >::operator= (
    const DeviceBCOOMatrix & other
) 
```




<hr>



### function operator= 

```C++
inline DeviceBCOOMatrix & muda::DeviceBCOOMatrix< Ty, 1 >::operator= (
    DeviceBCOOMatrix && other
) 
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::view () const
```




<hr>



### function viewer 

```C++
inline auto muda::DeviceBCOOMatrix< Ty, 1 >::viewer () 
```




<hr>



### function ~DeviceBCOOMatrix 

```C++
inline muda::DeviceBCOOMatrix< Ty, 1 >::~DeviceBCOOMatrix () 
```




<hr>
## Protected Attributes Documentation




### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::DeviceBCOOMatrix< Ty, 1 >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::DeviceBCOOMatrix< Ty, 1 >::m_legacy_descr;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename U, int M>
class muda::DeviceBCOOMatrix< Ty, 1 >::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_bcoo_matrix.h`

