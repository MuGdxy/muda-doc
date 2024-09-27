

# Class muda::Extent3D



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Extent3D**](classmuda_1_1_extent3_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Extent3D**](#function-extent3d-12) () <br> |
|  MUDA\_GENERIC | [**Extent3D**](#function-extent3d-22) (size\_t depth, size\_t height, size\_t width) <br> |
|  MUDA\_GENERIC cudaExtent | [**cuda\_extent**](#function-cuda_extent) () const<br> |
|  MUDA\_GENERIC size\_t | [**depth**](#function-depth) () const<br> |
|  MUDA\_GENERIC size\_t | [**height**](#function-height) () const<br> |
|  MUDA\_GENERIC bool | [**valid**](#function-valid) () const<br> |
|  MUDA\_GENERIC size\_t | [**width**](#function-width) () const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC [**Extent3D**](classmuda_1_1_extent3_d.md) | [**Zero**](#function-zero) () <br> |


























## Public Functions Documentation




### function Extent3D [1/2]

```C++
inline MUDA_GENERIC muda::Extent3D::Extent3D () 
```




<hr>



### function Extent3D [2/2]

```C++
inline MUDA_GENERIC muda::Extent3D::Extent3D (
    size_t depth,
    size_t height,
    size_t width
) 
```




<hr>



### function cuda\_extent 

```C++
template<typename T>
inline MUDA_GENERIC cudaExtent muda::Extent3D::cuda_extent () const
```




<hr>



### function depth 

```C++
inline MUDA_GENERIC size_t muda::Extent3D::depth () const
```




<hr>



### function height 

```C++
inline MUDA_GENERIC size_t muda::Extent3D::height () const
```




<hr>



### function valid 

```C++
inline MUDA_GENERIC bool muda::Extent3D::valid () const
```




<hr>



### function width 

```C++
inline MUDA_GENERIC size_t muda::Extent3D::width () const
```




<hr>
## Public Static Functions Documentation




### function Zero 

```C++
static inline MUDA_GENERIC Extent3D muda::Extent3D::Zero () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/extent.h`

