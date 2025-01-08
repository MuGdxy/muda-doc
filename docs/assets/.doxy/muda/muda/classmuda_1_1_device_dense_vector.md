

# Class muda::DeviceDenseVector

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceDenseVector**](#function-devicedensevector-15) () = default<br> |
|   | [**DeviceDenseVector**](#function-devicedensevector-25) (size\_t size) <br> |
|   | [**DeviceDenseVector**](#function-devicedensevector-35) (const [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) &) <br> |
|   | [**DeviceDenseVector**](#function-devicedensevector-45) ([**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) &&) <br> |
|   | [**DeviceDenseVector**](#function-devicedensevector-55) (const Eigen::VectorX&lt; T &gt; & vec) <br> |
|  auto | [**buffer\_view**](#function-buffer_view-12) () const<br> |
|  auto | [**buffer\_view**](#function-buffer_view-22) () <br> |
|  auto | [**capacity**](#function-capacity) () const<br> |
|  void | [**copy\_to**](#function-copy_to-12) (Eigen::VectorX&lt; T &gt; & vec) const<br> |
|  void | [**copy\_to**](#function-copy_to-22) (std::vector&lt; T &gt; & vec) const<br> |
|  [**CDenseVectorView**](classmuda_1_1_dense_vector_view_t.md)&lt; T &gt; | [**cview**](#function-cview) () const<br> |
|  cusparseDnVecDescr\_t | [**descr**](#function-descr) () const<br> |
|  void | [**fill**](#function-fill) (T value) <br> |
|   | [**operator CDenseVectorView&lt; T &gt;**](#function-operator-cdensevectorview<-t->) () const<br> |
|   | [**operator DenseVectorView&lt; T &gt;**](#function-operator-densevectorview<-t->) () <br> |
|  [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) & | [**operator=**](#function-operator) (const [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) &) <br> |
|  [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) & | [**operator=**](#function-operator_1) ([**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) &&) <br> |
|  [**DeviceDenseVector**](classmuda_1_1_device_dense_vector.md) & | [**operator=**](#function-operator_2) (const Eigen::VectorX&lt; T &gt; & vec) <br> |
|  void | [**reserve**](#function-reserve) (size\_t size) <br> |
|  void | [**resize**](#function-resize) (size\_t size) <br> |
|  auto | [**size**](#function-size) () const<br> |
|  [**CDenseVectorView**](classmuda_1_1_dense_vector_view_t.md)&lt; T &gt; | [**view**](#function-view-12) () const<br> |
|  [**DenseVectorView**](classmuda_1_1_dense_vector_view_t.md)&lt; T &gt; | [**view**](#function-view-22) () <br> |
|  [**DenseVectorViewer**](classmuda_1_1_dense_vector_viewer_t.md)&lt; T &gt; | [**viewer**](#function-viewer-12) () <br> |
|  [**CDenseVectorViewer**](classmuda_1_1_dense_vector_viewer_t.md)&lt; T &gt; | [**viewer**](#function-viewer-22) () const<br> |
|   | [**~DeviceDenseVector**](#function-devicedensevector) () <br> |




























## Public Functions Documentation




### function DeviceDenseVector [1/5]

```C++
muda::DeviceDenseVector::DeviceDenseVector () = default
```




<hr>



### function DeviceDenseVector [2/5]

```C++
muda::DeviceDenseVector::DeviceDenseVector (
    size_t size
) 
```




<hr>



### function DeviceDenseVector [3/5]

```C++
muda::DeviceDenseVector::DeviceDenseVector (
    const DeviceDenseVector &
) 
```




<hr>



### function DeviceDenseVector [4/5]

```C++
muda::DeviceDenseVector::DeviceDenseVector (
    DeviceDenseVector &&
) 
```




<hr>



### function DeviceDenseVector [5/5]

```C++
muda::DeviceDenseVector::DeviceDenseVector (
    const Eigen::VectorX< T > & vec
) 
```




<hr>



### function buffer\_view [1/2]

```C++
inline auto muda::DeviceDenseVector::buffer_view () const
```




<hr>



### function buffer\_view [2/2]

```C++
inline auto muda::DeviceDenseVector::buffer_view () 
```




<hr>



### function capacity 

```C++
inline auto muda::DeviceDenseVector::capacity () const
```




<hr>



### function copy\_to [1/2]

```C++
void muda::DeviceDenseVector::copy_to (
    Eigen::VectorX< T > & vec
) const
```




<hr>



### function copy\_to [2/2]

```C++
void muda::DeviceDenseVector::copy_to (
    std::vector< T > & vec
) const
```




<hr>



### function cview 

```C++
inline CDenseVectorView < T > muda::DeviceDenseVector::cview () const
```




<hr>



### function descr 

```C++
inline cusparseDnVecDescr_t muda::DeviceDenseVector::descr () const
```




<hr>



### function fill 

```C++
void muda::DeviceDenseVector::fill (
    T value
) 
```




<hr>



### function operator CDenseVectorView&lt; T &gt; 

```C++
inline muda::DeviceDenseVector::operator CDenseVectorView< T > () const
```




<hr>



### function operator DenseVectorView&lt; T &gt; 

```C++
inline muda::DeviceDenseVector::operator DenseVectorView< T > () 
```




<hr>



### function operator= 

```C++
DeviceDenseVector & muda::DeviceDenseVector::operator= (
    const DeviceDenseVector &
) 
```




<hr>



### function operator= 

```C++
DeviceDenseVector & muda::DeviceDenseVector::operator= (
    DeviceDenseVector &&
) 
```




<hr>



### function operator= 

```C++
DeviceDenseVector & muda::DeviceDenseVector::operator= (
    const Eigen::VectorX< T > & vec
) 
```




<hr>



### function reserve 

```C++
void muda::DeviceDenseVector::reserve (
    size_t size
) 
```




<hr>



### function resize 

```C++
void muda::DeviceDenseVector::resize (
    size_t size
) 
```




<hr>



### function size 

```C++
inline auto muda::DeviceDenseVector::size () const
```




<hr>



### function view [1/2]

```C++
CDenseVectorView < T > muda::DeviceDenseVector::view () const
```




<hr>



### function view [2/2]

```C++
DenseVectorView < T > muda::DeviceDenseVector::view () 
```




<hr>



### function viewer [1/2]

```C++
inline DenseVectorViewer < T > muda::DeviceDenseVector::viewer () 
```




<hr>



### function viewer [2/2]

```C++
inline CDenseVectorViewer < T > muda::DeviceDenseVector::viewer () const
```




<hr>



### function ~DeviceDenseVector 

```C++
muda::DeviceDenseVector::~DeviceDenseVector () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/device_dense_vector.h`

