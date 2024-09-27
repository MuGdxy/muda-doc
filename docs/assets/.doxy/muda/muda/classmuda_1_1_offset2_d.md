

# Class muda::Offset2D



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Offset2D**](classmuda_1_1_offset2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**Offset2D**](#function-offset2d-12) () <br> |
|  MUDA\_GENERIC | [**Offset2D**](#function-offset2d-22) (size\_t offset\_in\_height, size\_t offset\_in\_width) <br> |
|  MUDA\_GENERIC cudaPos | [**cuda\_pos**](#function-cuda_pos) () const<br> |
|  MUDA\_GENERIC size\_t | [**offset\_in\_height**](#function-offset_in_height) () const<br> |
|  MUDA\_GENERIC size\_t | [**offset\_in\_width**](#function-offset_in_width) () const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC [**Offset2D**](classmuda_1_1_offset2_d.md) | [**Zero**](#function-zero) () <br> |


























## Public Functions Documentation




### function Offset2D [1/2]

```C++
inline MUDA_GENERIC muda::Offset2D::Offset2D () 
```




<hr>



### function Offset2D [2/2]

```C++
inline MUDA_GENERIC muda::Offset2D::Offset2D (
    size_t offset_in_height,
    size_t offset_in_width
) 
```




<hr>



### function cuda\_pos 

```C++
template<typename T>
inline MUDA_GENERIC cudaPos muda::Offset2D::cuda_pos () const
```




<hr>



### function offset\_in\_height 

```C++
inline MUDA_GENERIC size_t muda::Offset2D::offset_in_height () const
```




<hr>



### function offset\_in\_width 

```C++
inline MUDA_GENERIC size_t muda::Offset2D::offset_in_width () const
```




<hr>
## Public Static Functions Documentation




### function Zero 

```C++
static inline MUDA_GENERIC Offset2D muda::Offset2D::Zero () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/extent.h`

