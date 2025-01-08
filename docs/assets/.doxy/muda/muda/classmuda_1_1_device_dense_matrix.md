

# Class muda::DeviceDenseMatrix

**template &lt;typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef Ty | [**value\_type**](#typedef-value_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceDenseMatrix**](#function-devicedensematrix-15) () = default<br> |
|   | [**DeviceDenseMatrix**](#function-devicedensematrix-25) (size\_t row, size\_t col, bool sym=false) <br> |
|   | [**DeviceDenseMatrix**](#function-devicedensematrix-35) (const [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) &) = default<br> |
|   | [**DeviceDenseMatrix**](#function-devicedensematrix-45) ([**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) &&) <br> |
|   | [**DeviceDenseMatrix**](#function-devicedensematrix-55) (const Eigen::MatrixX&lt; Ty &gt; &) <br> |
|  [**DenseMatrixView**](classmuda_1_1_dense_matrix_view_t.md)&lt; Ty &gt; | [**T**](#function-t-12) () <br> |
|  [**CDenseMatrixView**](classmuda_1_1_dense_matrix_view_t.md)&lt; Ty &gt; | [**T**](#function-t-22) () const<br> |
|  auto | [**buffer\_view**](#function-buffer_view-12) () const<br> |
|  auto | [**buffer\_view**](#function-buffer_view-22) () <br> |
|  size\_t | [**col**](#function-col) () const<br> |
|  void | [**copy\_to**](#function-copy_to-12) (Eigen::MatrixX&lt; Ty &gt; & mat) const<br> |
|  void | [**copy\_to**](#function-copy_to-22) (std::vector&lt; Ty &gt; & vec) const<br> |
|  [**CDenseMatrixView**](classmuda_1_1_dense_matrix_view_t.md)&lt; Ty &gt; | [**cview**](#function-cview) () const<br> |
|  [**CDenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; Ty &gt; | [**cviewer**](#function-cviewer) () const<br> |
|  void | [**fill**](#function-fill) (Ty value) <br> |
|   | [**operator CDenseMatrixView&lt; Ty &gt;**](#function-operator-cdensematrixview<-ty->) () const<br> |
|   | [**operator DenseMatrixView&lt; Ty &gt;**](#function-operator-densematrixview<-ty->) () <br> |
|  [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) & | [**operator=**](#function-operator) (const [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) &) = default<br> |
|  [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) & | [**operator=**](#function-operator_1) ([**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) &&) <br> |
|  [**DeviceDenseMatrix**](classmuda_1_1_device_dense_matrix.md) & | [**operator=**](#function-operator_2) (const Eigen::MatrixX&lt; Ty &gt; &) <br> |
|  void | [**reshape**](#function-reshape) (size\_t row, size\_t col) <br> |
|  size\_t | [**row**](#function-row) () const<br> |
|  void | [**sym**](#function-sym-12) (bool sym=true) <br> |
|  bool | [**sym**](#function-sym-22) () const<br> |
|  [**DenseMatrixView**](classmuda_1_1_dense_matrix_view_t.md)&lt; Ty &gt; | [**view**](#function-view-12) () <br> |
|  [**CDenseMatrixView**](classmuda_1_1_dense_matrix_view_t.md)&lt; Ty &gt; | [**view**](#function-view-22) () const<br> |
|  [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; Ty &gt; | [**viewer**](#function-viewer) () <br> |




























## Public Types Documentation




### typedef value\_type 

```C++
using muda::DeviceDenseMatrix< Ty >::value_type =  Ty;
```




<hr>
## Public Functions Documentation




### function DeviceDenseMatrix [1/5]

```C++
muda::DeviceDenseMatrix::DeviceDenseMatrix () = default
```




<hr>



### function DeviceDenseMatrix [2/5]

```C++
muda::DeviceDenseMatrix::DeviceDenseMatrix (
    size_t row,
    size_t col,
    bool sym=false
) 
```




<hr>



### function DeviceDenseMatrix [3/5]

```C++
muda::DeviceDenseMatrix::DeviceDenseMatrix (
    const DeviceDenseMatrix &
) = default
```




<hr>



### function DeviceDenseMatrix [4/5]

```C++
muda::DeviceDenseMatrix::DeviceDenseMatrix (
    DeviceDenseMatrix &&
) 
```




<hr>



### function DeviceDenseMatrix [5/5]

```C++
muda::DeviceDenseMatrix::DeviceDenseMatrix (
    const Eigen::MatrixX< Ty > &
) 
```




<hr>



### function T [1/2]

```C++
DenseMatrixView < Ty > muda::DeviceDenseMatrix::T () 
```




<hr>



### function T [2/2]

```C++
CDenseMatrixView < Ty > muda::DeviceDenseMatrix::T () const
```




<hr>



### function buffer\_view [1/2]

```C++
inline auto muda::DeviceDenseMatrix::buffer_view () const
```




<hr>



### function buffer\_view [2/2]

```C++
inline auto muda::DeviceDenseMatrix::buffer_view () 
```




<hr>



### function col 

```C++
inline size_t muda::DeviceDenseMatrix::col () const
```




<hr>



### function copy\_to [1/2]

```C++
void muda::DeviceDenseMatrix::copy_to (
    Eigen::MatrixX< Ty > & mat
) const
```




<hr>



### function copy\_to [2/2]

```C++
void muda::DeviceDenseMatrix::copy_to (
    std::vector< Ty > & vec
) const
```




<hr>



### function cview 

```C++
inline CDenseMatrixView < Ty > muda::DeviceDenseMatrix::cview () const
```




<hr>



### function cviewer 

```C++
inline CDenseMatrixViewer < Ty > muda::DeviceDenseMatrix::cviewer () const
```




<hr>



### function fill 

```C++
void muda::DeviceDenseMatrix::fill (
    Ty value
) 
```




<hr>



### function operator CDenseMatrixView&lt; Ty &gt; 

```C++
muda::DeviceDenseMatrix::operator CDenseMatrixView< Ty > () const
```




<hr>



### function operator DenseMatrixView&lt; Ty &gt; 

```C++
muda::DeviceDenseMatrix::operator DenseMatrixView< Ty > () 
```




<hr>



### function operator= 

```C++
DeviceDenseMatrix & muda::DeviceDenseMatrix::operator= (
    const DeviceDenseMatrix &
) = default
```




<hr>



### function operator= 

```C++
DeviceDenseMatrix & muda::DeviceDenseMatrix::operator= (
    DeviceDenseMatrix &&
) 
```




<hr>



### function operator= 

```C++
DeviceDenseMatrix & muda::DeviceDenseMatrix::operator= (
    const Eigen::MatrixX< Ty > &
) 
```




<hr>



### function reshape 

```C++
void muda::DeviceDenseMatrix::reshape (
    size_t row,
    size_t col
) 
```




<hr>



### function row 

```C++
inline size_t muda::DeviceDenseMatrix::row () const
```




<hr>



### function sym [1/2]

```C++
inline void muda::DeviceDenseMatrix::sym (
    bool sym=true
) 
```




<hr>



### function sym [2/2]

```C++
inline bool muda::DeviceDenseMatrix::sym () const
```




<hr>



### function view [1/2]

```C++
DenseMatrixView < Ty > muda::DeviceDenseMatrix::view () 
```




<hr>



### function view [2/2]

```C++
CDenseMatrixView < Ty > muda::DeviceDenseMatrix::view () const
```




<hr>



### function viewer 

```C++
inline DenseMatrixViewer < Ty > muda::DeviceDenseMatrix::viewer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_dense_matrix.h`

