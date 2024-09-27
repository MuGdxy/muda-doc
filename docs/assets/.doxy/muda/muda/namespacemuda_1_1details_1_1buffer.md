

# Namespace muda::details::buffer



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**buffer**](namespacemuda_1_1details_1_1buffer.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**BufferInfoAccessor**](classmuda_1_1details_1_1buffer_1_1_buffer_info_accessor.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST void | [**kernel\_assign**](#function-kernel_assign) (cudaStream\_t stream, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; dst, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_assign**](#function-kernel_assign) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; dst, [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_assign**](#function-kernel_assign) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; dst, [**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_assign**](#function-kernel_assign) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; dst, [**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_construct**](#function-kernel_construct) (cudaStream\_t stream, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; view) <br> |
|  MUDA\_HOST void | [**kernel\_construct**](#function-kernel_construct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; buffer\_view) <br> |
|  MUDA\_HOST void | [**kernel\_construct**](#function-kernel_construct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; buffer\_view) <br> |
|  MUDA\_HOST void | [**kernel\_construct**](#function-kernel_construct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; buffer\_view) <br> |
|  MUDA\_HOST void | [**kernel\_copy\_construct**](#function-kernel_copy_construct) (cudaStream\_t stream, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; dst, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_copy\_construct**](#function-kernel_copy_construct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; dst, [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_copy\_construct**](#function-kernel_copy_construct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; dst, [**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_copy\_construct**](#function-kernel_copy_construct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; dst, [**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST void | [**kernel\_destruct**](#function-kernel_destruct) (cudaStream\_t stream, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; view) <br> |
|  MUDA\_HOST void | [**kernel\_destruct**](#function-kernel_destruct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; buffer\_view) <br> |
|  MUDA\_HOST void | [**kernel\_destruct**](#function-kernel_destruct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; buffer\_view) <br> |
|  MUDA\_HOST void | [**kernel\_destruct**](#function-kernel_destruct) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; buffer\_view) <br> |
|  MUDA\_HOST void | [**kernel\_fill**](#function-kernel_fill) (cudaStream\_t stream, [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; dst, const T & val) <br> |
|  MUDA\_HOST void | [**kernel\_fill**](#function-kernel_fill) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; dst, const T & val) <br> |
|  MUDA\_HOST void | [**kernel\_fill**](#function-kernel_fill) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; dst, const T & val) <br> |
|  MUDA\_HOST void | [**kernel\_fill**](#function-kernel_fill) (int grid\_dim, int block\_dim, cudaStream\_t stream, [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; dst, const T & val) <br> |
|  MUDA\_INLINE bool | [**less**](#function-less) (bool b, size\_t l, size\_t r) <br> |
|  MUDA\_INLINE bool | [**less**](#function-less) (std::bitset&lt; N &gt; mask, const std::array&lt; size\_t, N &gt; & lhs, const std::array&lt; size\_t, N &gt; & rhs) <br> |
|  MUDA\_INLINE MUDA\_HOST [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; | [**reserve\_1d**](#function-reserve_1d) (cudaStream\_t stream, size\_t size) <br> |
|  MUDA\_INLINE MUDA\_HOST [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; | [**reserve\_2d**](#function-reserve_2d) (cudaStream\_t stream, [**Extent2D**](classmuda_1_1_extent2_d.md) extent) <br> |
|  MUDA\_INLINE MUDA\_HOST [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; | [**reserve\_3d**](#function-reserve_3d) (cudaStream\_t stream, [**Extent3D**](classmuda_1_1_extent3_d.md) extent) <br> |
|  MUDA\_INLINE void | [**swap**](#function-swap) (bool b, size\_t & l, size\_t & r) <br> |
|  MUDA\_INLINE void | [**swap**](#function-swap) (std::bitset&lt; N &gt; mask, std::array&lt; size\_t, N &gt; & lhs, std::array&lt; size\_t, N &gt; & rhs) <br> |




























## Public Functions Documentation




### function kernel\_assign 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_assign (
    cudaStream_t stream,
    VarView < T > dst,
    CVarView < T > src
) 
```




<hr>



### function kernel\_assign 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_assign (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    BufferView < T > dst,
    CBufferView < T > src
) 
```




<hr>



### function kernel\_assign 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_assign (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer2DView < T > dst,
    CBuffer2DView < T > src
) 
```




<hr>



### function kernel\_assign 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_assign (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer3DView < T > dst,
    CBuffer3DView < T > src
) 
```




<hr>



### function kernel\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_construct (
    cudaStream_t stream,
    VarView < T > view
) 
```




<hr>



### function kernel\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_construct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    BufferView < T > buffer_view
) 
```




<hr>



### function kernel\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_construct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer2DView < T > buffer_view
) 
```




<hr>



### function kernel\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_construct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer3DView < T > buffer_view
) 
```




<hr>



### function kernel\_copy\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_copy_construct (
    cudaStream_t stream,
    VarView < T > dst,
    CVarView < T > src
) 
```




<hr>



### function kernel\_copy\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_copy_construct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    BufferView < T > dst,
    CBufferView < T > src
) 
```




<hr>



### function kernel\_copy\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_copy_construct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer2DView < T > dst,
    CBuffer2DView < T > src
) 
```




<hr>



### function kernel\_copy\_construct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_copy_construct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer3DView < T > dst,
    CBuffer3DView < T > src
) 
```




<hr>



### function kernel\_destruct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_destruct (
    cudaStream_t stream,
    VarView < T > view
) 
```




<hr>



### function kernel\_destruct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_destruct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    BufferView < T > buffer_view
) 
```




<hr>



### function kernel\_destruct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_destruct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer2DView < T > buffer_view
) 
```




<hr>



### function kernel\_destruct 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_destruct (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer3DView < T > buffer_view
) 
```




<hr>



### function kernel\_fill 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_fill (
    cudaStream_t stream,
    VarView < T > dst,
    const T & val
) 
```




<hr>



### function kernel\_fill 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_fill (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    BufferView < T > dst,
    const T & val
) 
```




<hr>



### function kernel\_fill 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_fill (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer2DView < T > dst,
    const T & val
) 
```




<hr>



### function kernel\_fill 

```C++
template<typename T>
MUDA_HOST void muda::details::buffer::kernel_fill (
    int grid_dim,
    int block_dim,
    cudaStream_t stream,
    Buffer3DView < T > dst,
    const T & val
) 
```




<hr>



### function less 

```C++
MUDA_INLINE bool muda::details::buffer::less (
    bool b,
    size_t l,
    size_t r
) 
```




<hr>



### function less 

```C++
template<size_t N>
MUDA_INLINE bool muda::details::buffer::less (
    std::bitset< N > mask,
    const std::array< size_t, N > & lhs,
    const std::array< size_t, N > & rhs
) 
```




<hr>



### function reserve\_1d 

```C++
template<typename T>
MUDA_INLINE MUDA_HOST BufferView < T > muda::details::buffer::reserve_1d (
    cudaStream_t stream,
    size_t size
) 
```




<hr>



### function reserve\_2d 

```C++
template<typename T>
MUDA_INLINE MUDA_HOST Buffer2DView < T > muda::details::buffer::reserve_2d (
    cudaStream_t stream,
    Extent2D extent
) 
```




<hr>



### function reserve\_3d 

```C++
template<typename T>
MUDA_INLINE MUDA_HOST Buffer3DView < T > muda::details::buffer::reserve_3d (
    cudaStream_t stream,
    Extent3D extent
) 
```




<hr>



### function swap 

```C++
MUDA_INLINE void muda::details::buffer::swap (
    bool b,
    size_t & l,
    size_t & r
) 
```




<hr>



### function swap 

```C++
template<size_t N>
MUDA_INLINE void muda::details::buffer::swap (
    std::bitset< N > mask,
    std::array< size_t, N > & lhs,
    std::array< size_t, N > & rhs
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/agent/kernel_assign.h`

