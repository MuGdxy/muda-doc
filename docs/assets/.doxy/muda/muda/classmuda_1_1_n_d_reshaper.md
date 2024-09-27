

# Class muda::NDReshaper



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**NDReshaper**](classmuda_1_1_n_d_reshaper.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST void | [**reserve**](#function-reserve-13) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer, size\_t new\_capacity) <br> |
|  MUDA\_HOST void | [**reserve**](#function-reserve-23) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer, [**Extent2D**](classmuda_1_1_extent2_d.md) new\_capacity) <br> |
|  MUDA\_HOST void | [**reserve**](#function-reserve-33) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer, [**Extent3D**](classmuda_1_1_extent3_d.md) new\_capacity) <br> |
|  MUDA\_HOST void | [**resize**](#function-resize-13) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer, size\_t new\_size, FConstruct && fct) <br> |
|  MUDA\_HOST void | [**resize**](#function-resize-23) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer, [**Extent2D**](classmuda_1_1_extent2_d.md) new\_extent, FConstruct && fct) <br> |
|  MUDA\_HOST void | [**resize**](#function-resize-33) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer, [**Extent3D**](classmuda_1_1_extent3_d.md) new\_extent, FConstruct && fct) <br> |
|  MUDA\_HOST void | [**shrink\_to\_fit**](#function-shrink_to_fit-13) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST void | [**shrink\_to\_fit**](#function-shrink_to_fit-23) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST void | [**shrink\_to\_fit**](#function-shrink_to_fit-33) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer) <br> |


























## Public Static Functions Documentation




### function reserve [1/3]

```C++
template<typename T>
static MUDA_HOST void muda::NDReshaper::reserve (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer < T > & buffer,
    size_t new_capacity
) 
```




<hr>



### function reserve [2/3]

```C++
template<typename T>
static MUDA_HOST void muda::NDReshaper::reserve (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer2D < T > & buffer,
    Extent2D new_capacity
) 
```




<hr>



### function reserve [3/3]

```C++
template<typename T>
static MUDA_HOST void muda::NDReshaper::reserve (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer3D < T > & buffer,
    Extent3D new_capacity
) 
```




<hr>



### function resize [1/3]

```C++
template<typename T, typename FConstruct>
static MUDA_HOST void muda::NDReshaper::resize (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer < T > & buffer,
    size_t new_size,
    FConstruct && fct
) 
```




<hr>



### function resize [2/3]

```C++
template<typename T, typename FConstruct>
static MUDA_HOST void muda::NDReshaper::resize (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer2D < T > & buffer,
    Extent2D new_extent,
    FConstruct && fct
) 
```




<hr>



### function resize [3/3]

```C++
template<typename T, typename FConstruct>
static MUDA_HOST void muda::NDReshaper::resize (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer3D < T > & buffer,
    Extent3D new_extent,
    FConstruct && fct
) 
```




<hr>



### function shrink\_to\_fit [1/3]

```C++
template<typename T>
static MUDA_HOST void muda::NDReshaper::shrink_to_fit (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer < T > & buffer
) 
```




<hr>



### function shrink\_to\_fit [2/3]

```C++
template<typename T>
static MUDA_HOST void muda::NDReshaper::shrink_to_fit (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer2D < T > & buffer
) 
```




<hr>



### function shrink\_to\_fit [3/3]

```C++
template<typename T>
static MUDA_HOST void muda::NDReshaper::shrink_to_fit (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    DeviceBuffer3D < T > & buffer
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/reshape_nd/nd_reshaper.h`

