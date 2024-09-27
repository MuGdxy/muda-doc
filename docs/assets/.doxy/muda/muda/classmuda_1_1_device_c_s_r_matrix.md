

# Class muda::DeviceCSRMatrix

**template &lt;typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_col**](#variable-m_col)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_col\_indices**](#variable-m_col_indices)  <br> |
|  cusparseSpMatDescr\_t | [**m\_descr**](#variable-m_descr)   = = nullptr<br> |
|  cusparseMatDescr\_t | [**m\_legacy\_descr**](#variable-m_legacy_descr)   = = nullptr<br> |
|  int | [**m\_row**](#variable-m_row)   = = 0<br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_row\_offsets**](#variable-m_row_offsets)  <br> |
|  [**muda::DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; Ty &gt; | [**m\_values**](#variable-m_values)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceCSRMatrix**](#function-devicecsrmatrix-13) () = default<br> |
|   | [**DeviceCSRMatrix**](#function-devicecsrmatrix-23) (const [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md) &) <br> |
|   | [**DeviceCSRMatrix**](#function-devicecsrmatrix-33) ([**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md) &&) noexcept<br> |
|  auto | [**T**](#function-t-12) () const<br> |
|  auto | [**T**](#function-t-22) () <br> |
|  void | [**clear**](#function-clear) () <br> |
|  auto | [**col\_indices**](#function-col_indices-12) () <br> |
|  auto | [**col\_indices**](#function-col_indices-22) () const<br> |
|  auto | [**cols**](#function-cols) () const<br> |
|  auto | [**cview**](#function-cview) () const<br> |
|  cusparseSpMatDescr\_t | [**descr**](#function-descr) () const<br> |
|  cusparseMatDescr\_t | [**legacy\_descr**](#function-legacy_descr) () const<br> |
|  auto | [**non\_zeros**](#function-non_zeros) () const<br> |
|   | [**operator CCSRMatrixView&lt; Ty &gt;**](#function-operator-ccsrmatrixview<-ty->) () const<br> |
|   | [**operator CSRMatrixView&lt; Ty &gt;**](#function-operator-csrmatrixview<-ty->) () <br> |
|  [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md) &) <br> |
|  [**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceCSRMatrix**](classmuda_1_1_device_c_s_r_matrix.md) &&) noexcept<br> |
|  void | [**reserve**](#function-reserve) (int non\_zeros) <br> |
|  void | [**reshape**](#function-reshape) (int row, int col) <br> |
|  auto | [**row\_offsets**](#function-row_offsets-12) () <br> |
|  auto | [**row\_offsets**](#function-row_offsets-22) () const<br> |
|  auto | [**rows**](#function-rows) () const<br> |
|  auto | [**values**](#function-values-12) () <br> |
|  auto | [**values**](#function-values-22) () const<br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|   | [**~DeviceCSRMatrix**](#function-devicecsrmatrix) () <br> |




























## Public Attributes Documentation




### variable m\_col 

```C++
int muda::DeviceCSRMatrix< Ty >::m_col;
```




<hr>



### variable m\_col\_indices 

```C++
muda::DeviceBuffer<int> muda::DeviceCSRMatrix< Ty >::m_col_indices;
```




<hr>



### variable m\_descr 

```C++
cusparseSpMatDescr_t muda::DeviceCSRMatrix< Ty >::m_descr;
```




<hr>



### variable m\_legacy\_descr 

```C++
cusparseMatDescr_t muda::DeviceCSRMatrix< Ty >::m_legacy_descr;
```




<hr>



### variable m\_row 

```C++
int muda::DeviceCSRMatrix< Ty >::m_row;
```




<hr>



### variable m\_row\_offsets 

```C++
muda::DeviceBuffer<int> muda::DeviceCSRMatrix< Ty >::m_row_offsets;
```




<hr>



### variable m\_values 

```C++
muda::DeviceBuffer<Ty> muda::DeviceCSRMatrix< Ty >::m_values;
```




<hr>
## Public Functions Documentation




### function DeviceCSRMatrix [1/3]

```C++
muda::DeviceCSRMatrix::DeviceCSRMatrix () = default
```




<hr>



### function DeviceCSRMatrix [2/3]

```C++
muda::DeviceCSRMatrix::DeviceCSRMatrix (
    const DeviceCSRMatrix &
) 
```




<hr>



### function DeviceCSRMatrix [3/3]

```C++
muda::DeviceCSRMatrix::DeviceCSRMatrix (
    DeviceCSRMatrix &&
) noexcept
```




<hr>



### function T [1/2]

```C++
inline auto muda::DeviceCSRMatrix::T () const
```




<hr>



### function T [2/2]

```C++
inline auto muda::DeviceCSRMatrix::T () 
```




<hr>



### function clear 

```C++
void muda::DeviceCSRMatrix::clear () 
```




<hr>



### function col\_indices [1/2]

```C++
inline auto muda::DeviceCSRMatrix::col_indices () 
```




<hr>



### function col\_indices [2/2]

```C++
inline auto muda::DeviceCSRMatrix::col_indices () const
```




<hr>



### function cols 

```C++
inline auto muda::DeviceCSRMatrix::cols () const
```




<hr>



### function cview 

```C++
inline auto muda::DeviceCSRMatrix::cview () const
```




<hr>



### function descr 

```C++
cusparseSpMatDescr_t muda::DeviceCSRMatrix::descr () const
```




<hr>



### function legacy\_descr 

```C++
cusparseMatDescr_t muda::DeviceCSRMatrix::legacy_descr () const
```




<hr>



### function non\_zeros 

```C++
inline auto muda::DeviceCSRMatrix::non_zeros () const
```




<hr>



### function operator CCSRMatrixView&lt; Ty &gt; 

```C++
inline muda::DeviceCSRMatrix::operator CCSRMatrixView< Ty > () const
```




<hr>



### function operator CSRMatrixView&lt; Ty &gt; 

```C++
inline muda::DeviceCSRMatrix::operator CSRMatrixView< Ty > () 
```




<hr>



### function operator= 

```C++
DeviceCSRMatrix & muda::DeviceCSRMatrix::operator= (
    const DeviceCSRMatrix &
) 
```




<hr>



### function operator= 

```C++
DeviceCSRMatrix & muda::DeviceCSRMatrix::operator= (
    DeviceCSRMatrix &&
) noexcept
```




<hr>



### function reserve 

```C++
void muda::DeviceCSRMatrix::reserve (
    int non_zeros
) 
```




<hr>



### function reshape 

```C++
void muda::DeviceCSRMatrix::reshape (
    int row,
    int col
) 
```




<hr>



### function row\_offsets [1/2]

```C++
inline auto muda::DeviceCSRMatrix::row_offsets () 
```




<hr>



### function row\_offsets [2/2]

```C++
inline auto muda::DeviceCSRMatrix::row_offsets () const
```




<hr>



### function rows 

```C++
inline auto muda::DeviceCSRMatrix::rows () const
```




<hr>



### function values [1/2]

```C++
inline auto muda::DeviceCSRMatrix::values () 
```




<hr>



### function values [2/2]

```C++
inline auto muda::DeviceCSRMatrix::values () const
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceCSRMatrix::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceCSRMatrix::view () const
```




<hr>



### function ~DeviceCSRMatrix 

```C++
muda::DeviceCSRMatrix::~DeviceCSRMatrix () 
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename T, int N>
class muda::DeviceCSRMatrix::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_csr_matrix.h`

