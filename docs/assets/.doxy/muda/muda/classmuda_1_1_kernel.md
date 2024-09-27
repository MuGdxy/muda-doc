

# Class muda::Kernel

**template &lt;typename F&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Kernel**](classmuda_1_1_kernel.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-18) (dim3 grid\_dim, dim3 m\_block\_dim, size\_t shared\_memory\_size, cudaStream\_t stream, F f) <br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-28) (F f) <br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-38) (dim3 grid\_dim, dim3 m\_block\_dim, F f) <br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-48) (dim3 grid\_dim, dim3 m\_block\_dim, size\_t shared\_memory\_size, F f) <br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-58) (dim3 grid\_dim, dim3 m\_block\_dim, cudaStream\_t stream, F f) <br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-68) (cudaStream\_t stream, F f) <br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-78) (const [**Kernel**](classmuda_1_1_kernel.md) &) = delete<br> |
|  MUDA\_GENERIC | [**Kernel**](#function-kernel-88) ([**Kernel**](classmuda_1_1_kernel.md) &&) = delete<br> |
|  MUDA\_GENERIC void | [**operator()**](#function-operator()) (Args &&... args) <br> |
|  MUDA\_GENERIC [**Kernel**](classmuda_1_1_kernel.md) & | [**operator=**](#function-operator) (const [**Kernel**](classmuda_1_1_kernel.md) &) = delete<br> |
|  MUDA\_GENERIC [**Kernel**](classmuda_1_1_kernel.md) & | [**operator=**](#function-operator_1) ([**Kernel**](classmuda_1_1_kernel.md) &&) = delete<br> |




























## Public Functions Documentation




### function Kernel [1/8]

```C++
inline MUDA_GENERIC muda::Kernel::Kernel (
    dim3 grid_dim,
    dim3 m_block_dim,
    size_t shared_memory_size,
    cudaStream_t stream,
    F f
) 
```




<hr>



### function Kernel [2/8]

```C++
inline MUDA_GENERIC muda::Kernel::Kernel (
    F f
) 
```




<hr>



### function Kernel [3/8]

```C++
inline MUDA_GENERIC muda::Kernel::Kernel (
    dim3 grid_dim,
    dim3 m_block_dim,
    F f
) 
```




<hr>



### function Kernel [4/8]

```C++
inline MUDA_GENERIC muda::Kernel::Kernel (
    dim3 grid_dim,
    dim3 m_block_dim,
    size_t shared_memory_size,
    F f
) 
```




<hr>



### function Kernel [5/8]

```C++
inline MUDA_GENERIC muda::Kernel::Kernel (
    dim3 grid_dim,
    dim3 m_block_dim,
    cudaStream_t stream,
    F f
) 
```




<hr>



### function Kernel [6/8]

```C++
inline MUDA_GENERIC muda::Kernel::Kernel (
    cudaStream_t stream,
    F f
) 
```




<hr>



### function Kernel [7/8]

```C++
MUDA_GENERIC muda::Kernel::Kernel (
    const Kernel &
) = delete
```




<hr>



### function Kernel [8/8]

```C++
MUDA_GENERIC muda::Kernel::Kernel (
    Kernel &&
) = delete
```




<hr>



### function operator() 

```C++
template<typename... Args>
inline MUDA_GENERIC void muda::Kernel::operator() (
    Args &&... args
) 
```




<hr>



### function operator= 

```C++
MUDA_GENERIC Kernel & muda::Kernel::operator= (
    const Kernel &
) = delete
```




<hr>



### function operator= 

```C++
MUDA_GENERIC Kernel & muda::Kernel::operator= (
    Kernel &&
) = delete
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/kernel.h`

