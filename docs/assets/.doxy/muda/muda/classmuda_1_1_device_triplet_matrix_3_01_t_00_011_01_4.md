

# Class muda::DeviceTripletMatrix&lt; T, 1 &gt;

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceTripletMatrix&lt; T, 1 &gt;**](classmuda_1_1_device_triplet_matrix_3_01_t_00_011_01_4.md)










































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
|  auto | [**cviewer**](#function-cviewer) () const<br> |
|   | [**operator CTripletMatrixView&lt; T, 1 &gt;**](#function-operator-ctripletmatrixview<-t,-1->) () const<br> |
|   | [**operator TripletMatrixView&lt; T, 1 &gt;**](#function-operator-tripletmatrixview<-t,-1->) () <br> |
|  [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &) = default<br> |
|  [**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceTripletMatrix**](classmuda_1_1_device_triplet_matrix.md) &&) = default<br> |
|  void | [**reserve\_triplets**](#function-reserve_triplets) (size\_t nonzero\_count) <br> |
|  void | [**reshape**](#function-reshape) (int row, int col) <br> |
|  void | [**resize**](#function-resize) (int row, int col, size\_t nonzero\_count) <br> |
|  void | [**resize\_triplets**](#function-resize_triplets) (size\_t nonzero\_count) <br> |
|  auto | [**row\_indices**](#function-row_indices-12) () <br> |
|  auto | [**row\_indices**](#function-row_indices-22) () const<br> |
|  auto | [**rows**](#function-rows) () const<br> |
|  auto | [**triplet\_count**](#function-triplet_count) () const<br> |
|  auto | [**values**](#function-values-12) () <br> |
|  auto | [**values**](#function-values-22) () const<br> |
|  auto | [**view**](#function-view-12) () const<br> |
|  auto | [**view**](#function-view-22) () <br> |
|  auto | [**viewer**](#function-viewer) () <br> |
|   | [**~DeviceTripletMatrix**](#function-devicetripletmatrix) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  constexpr int | [**block\_size**](#function-block_size) () <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_col\_indices**](#variable-m_col_indices)  <br> |
|  int | [**m\_cols**](#variable-m_cols)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**m\_row\_indices**](#variable-m_row_indices)  <br> |
|  int | [**m\_rows**](#variable-m_rows)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; | [**m\_values**](#variable-m_values)  <br> |




















## Public Functions Documentation




### function DeviceTripletMatrix [1/3]

```C++
muda::DeviceTripletMatrix< T, 1 >::DeviceTripletMatrix () = default
```




<hr>



### function DeviceTripletMatrix [2/3]

```C++
muda::DeviceTripletMatrix< T, 1 >::DeviceTripletMatrix (
    const DeviceTripletMatrix &
) = default
```




<hr>



### function DeviceTripletMatrix [3/3]

```C++
muda::DeviceTripletMatrix< T, 1 >::DeviceTripletMatrix (
    DeviceTripletMatrix &&
) = default
```




<hr>



### function clear 

```C++
inline void muda::DeviceTripletMatrix< T, 1 >::clear () 
```




<hr>



### function col\_indices [1/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::col_indices () 
```




<hr>



### function col\_indices [2/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::col_indices () const
```




<hr>



### function cols 

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::cols () const
```




<hr>



### function cviewer 

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::cviewer () const
```




<hr>



### function operator CTripletMatrixView&lt; T, 1 &gt; 

```C++
inline muda::DeviceTripletMatrix< T, 1 >::operator CTripletMatrixView< T, 1 > () const
```




<hr>



### function operator TripletMatrixView&lt; T, 1 &gt; 

```C++
inline muda::DeviceTripletMatrix< T, 1 >::operator TripletMatrixView< T, 1 > () 
```




<hr>



### function operator= 

```C++
DeviceTripletMatrix & muda::DeviceTripletMatrix< T, 1 >::operator= (
    const DeviceTripletMatrix &
) = default
```




<hr>



### function operator= 

```C++
DeviceTripletMatrix & muda::DeviceTripletMatrix< T, 1 >::operator= (
    DeviceTripletMatrix &&
) = default
```




<hr>



### function reserve\_triplets 

```C++
inline void muda::DeviceTripletMatrix< T, 1 >::reserve_triplets (
    size_t nonzero_count
) 
```




<hr>



### function reshape 

```C++
inline void muda::DeviceTripletMatrix< T, 1 >::reshape (
    int row,
    int col
) 
```




<hr>



### function resize 

```C++
inline void muda::DeviceTripletMatrix< T, 1 >::resize (
    int row,
    int col,
    size_t nonzero_count
) 
```




<hr>



### function resize\_triplets 

```C++
inline void muda::DeviceTripletMatrix< T, 1 >::resize_triplets (
    size_t nonzero_count
) 
```




<hr>



### function row\_indices [1/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::row_indices () 
```




<hr>



### function row\_indices [2/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::row_indices () const
```




<hr>



### function rows 

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::rows () const
```




<hr>



### function triplet\_count 

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::triplet_count () const
```




<hr>



### function values [1/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::values () 
```




<hr>



### function values [2/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::values () const
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::view () const
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::view () 
```




<hr>



### function viewer 

```C++
inline auto muda::DeviceTripletMatrix< T, 1 >::viewer () 
```




<hr>



### function ~DeviceTripletMatrix 

```C++
muda::DeviceTripletMatrix< T, 1 >::~DeviceTripletMatrix () = default
```




<hr>
## Public Static Functions Documentation




### function block\_size 

```C++
static inline constexpr int muda::DeviceTripletMatrix< T, 1 >::block_size () 
```




<hr>
## Protected Attributes Documentation




### variable m\_col\_indices 

```C++
DeviceBuffer<int> muda::DeviceTripletMatrix< T, 1 >::m_col_indices;
```




<hr>



### variable m\_cols 

```C++
int muda::DeviceTripletMatrix< T, 1 >::m_cols;
```




<hr>



### variable m\_row\_indices 

```C++
DeviceBuffer<int> muda::DeviceTripletMatrix< T, 1 >::m_row_indices;
```




<hr>



### variable m\_rows 

```C++
int muda::DeviceTripletMatrix< T, 1 >::m_rows;
```




<hr>



### variable m\_values 

```C++
DeviceBuffer<T> muda::DeviceTripletMatrix< T, 1 >::m_values;
```




<hr>## Friends Documentation





### friend MatrixFormatConverter 

```C++
template<typename U, int M>
class muda::DeviceTripletMatrix< T, 1 >::MatrixFormatConverter (
    details::MatrixFormatConverter
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_triplet_matrix.h`

