

# Class muda::Extent2D



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Extent2D**](classmuda_1_1_extent2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Extent2D**](#function-extent2d-12) () <br> |
|  MUDA\_GENERIC | [**Extent2D**](#function-extent2d-22) (size\_t height, size\_t width) <br> |
|  MUDA\_GENERIC cudaExtent | [**cuda\_extent**](#function-cuda_extent) () const<br> |
|  MUDA\_GENERIC size\_t | [**height**](#function-height) () const<br> |
|  MUDA\_GENERIC bool | [**valid**](#function-valid) () const<br> |
|  MUDA\_GENERIC size\_t | [**width**](#function-width) () const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC [**Extent2D**](classmuda_1_1_extent2_d.md) | [**Zero**](#function-zero) () <br> |


























## Public Functions Documentation




### function Extent2D [1/2]

```C++
inline MUDA_GENERIC muda::Extent2D::Extent2D () 
```




<hr>



### function Extent2D [2/2]

```C++
inline MUDA_GENERIC muda::Extent2D::Extent2D (
    size_t height,
    size_t width
) 
```




<hr>



### function cuda\_extent 

```C++
template<typename T>
inline MUDA_GENERIC cudaExtent muda::Extent2D::cuda_extent () const
```




<hr>



### function height 

```C++
inline MUDA_GENERIC size_t muda::Extent2D::height () const
```




<hr>



### function valid 

```C++
inline MUDA_GENERIC bool muda::Extent2D::valid () const
```




<hr>



### function width 

```C++
inline MUDA_GENERIC size_t muda::Extent2D::width () const
```




<hr>
## Public Static Functions Documentation




### function Zero 

```C++
static inline MUDA_GENERIC Extent2D muda::Extent2D::Zero () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/extent.h`

