

# Class muda::DeviceVector

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceVector**](classmuda_1_1_device_vector.md)








Inherits the following classes: thrust::device_vector< T, thrust::device_allocator< T > >














## Public Types

| Type | Name |
| ---: | :--- |
| typedef thrust::device\_vector&lt; T, thrust::device\_allocator&lt; T &gt; &gt; | [**Base**](#typedef-base)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**copy\_to**](#function-copy_to) (std::vector&lt; T &gt; & v) const<br> |
|  auto | [**cviewer**](#function-cviewer) () const<br> |
|   | [**operator BufferView&lt; T &gt;**](#function-operator-bufferview<-t->) () const<br> |
|   | [**operator CBufferView&lt; T &gt;**](#function-operator-cbufferview<-t->) () const<br> |
|  [**DeviceVector**](classmuda_1_1_device_vector.md) & | [**operator=**](#function-operator) ([**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; v) <br> |
|  auto | [**view**](#function-view-12) () <br> |
|  auto | [**view**](#function-view-22) () const<br> |
|  auto | [**viewer**](#function-viewer) () <br> |




























## Public Types Documentation




### typedef Base 

```C++
using muda::DeviceVector< T >::Base =  thrust::device_vector<T, thrust::device_allocator<T> >;
```




<hr>
## Public Functions Documentation




### function copy\_to 

```C++
inline void muda::DeviceVector::copy_to (
    std::vector< T > & v
) const
```




<hr>



### function cviewer 

```C++
inline auto muda::DeviceVector::cviewer () const
```




<hr>



### function operator BufferView&lt; T &gt; 

```C++
inline muda::DeviceVector::operator BufferView< T > () const
```




<hr>



### function operator CBufferView&lt; T &gt; 

```C++
inline muda::DeviceVector::operator CBufferView< T > () const
```




<hr>



### function operator= 

```C++
inline DeviceVector & muda::DeviceVector::operator= (
    CBufferView < T > v
) 
```




<hr>



### function view [1/2]

```C++
inline auto muda::DeviceVector::view () 
```




<hr>



### function view [2/2]

```C++
inline auto muda::DeviceVector::view () const
```




<hr>



### function viewer 

```C++
inline auto muda::DeviceVector::viewer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/container/vector.h`

