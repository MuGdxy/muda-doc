

# Class muda::LinearSystemHandles



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**LinearSystemHandles**](#function-linearsystemhandles) (cudaStream\_t s) <br> |
|  cublasHandle\_t | [**cublas**](#function-cublas) () const<br> |
|  cusolverDnHandle\_t | [**cusolver\_dn**](#function-cusolver_dn) () const<br> |
|  cusolverSpHandle\_t | [**cusolver\_sp**](#function-cusolver_sp) () const<br> |
|  cusparseHandle\_t | [**cusparse**](#function-cusparse) () const<br> |
|  auto | [**reserve\_ratio**](#function-reserve_ratio) () const<br> |
|  MUDA\_INLINE void | [**set\_pointer\_mode\_device**](#function-set_pointer_mode_device) () <br> |
|  MUDA\_INLINE void | [**set\_pointer\_mode\_host**](#function-set_pointer_mode_host) () <br> |
|  void | [**stream**](#function-stream-12) (cudaStream\_t s) <br> |
|  cudaStream\_t | [**stream**](#function-stream-22) () const<br> |
|   | [**~LinearSystemHandles**](#function-linearsystemhandles) () <br> |




























## Public Functions Documentation




### function LinearSystemHandles 

```C++
inline muda::LinearSystemHandles::LinearSystemHandles (
    cudaStream_t s
) 
```




<hr>



### function cublas 

```C++
inline cublasHandle_t muda::LinearSystemHandles::cublas () const
```




<hr>



### function cusolver\_dn 

```C++
inline cusolverDnHandle_t muda::LinearSystemHandles::cusolver_dn () const
```




<hr>



### function cusolver\_sp 

```C++
inline cusolverSpHandle_t muda::LinearSystemHandles::cusolver_sp () const
```




<hr>



### function cusparse 

```C++
inline cusparseHandle_t muda::LinearSystemHandles::cusparse () const
```




<hr>



### function reserve\_ratio 

```C++
inline auto muda::LinearSystemHandles::reserve_ratio () const
```




<hr>



### function set\_pointer\_mode\_device 

```C++
inline MUDA_INLINE void muda::LinearSystemHandles::set_pointer_mode_device () 
```




<hr>



### function set\_pointer\_mode\_host 

```C++
inline MUDA_INLINE void muda::LinearSystemHandles::set_pointer_mode_host () 
```




<hr>



### function stream [1/2]

```C++
inline void muda::LinearSystemHandles::stream (
    cudaStream_t s
) 
```




<hr>



### function stream [2/2]

```C++
inline cudaStream_t muda::LinearSystemHandles::stream () const
```




<hr>



### function ~LinearSystemHandles 

```C++
inline muda::LinearSystemHandles::~LinearSystemHandles () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/linear_system_handles.h`

