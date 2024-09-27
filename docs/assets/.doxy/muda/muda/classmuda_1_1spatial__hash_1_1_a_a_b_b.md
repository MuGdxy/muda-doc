

# Class muda::spatial\_hash::AABB



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  Vector3 | [**max**](#variable-max)  <br> |
|  Vector3 | [**min**](#variable-min)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**AABB**](#function-aabb-12) (const Vector3 & min, const Vector3 & max) <br> |
|  MUDA\_GENERIC | [**AABB**](#function-aabb-22) (const [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) & l, const [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) & r) <br> |
|  MUDA\_GENERIC Vector3 | [**center**](#function-center) () const<br> |
|  MUDA\_GENERIC float | [**radius**](#function-radius) () const<br> |




























## Public Attributes Documentation




### variable max 

```C++
Vector3 muda::spatial_hash::AABB::max;
```




<hr>



### variable min 

```C++
Vector3 muda::spatial_hash::AABB::min;
```




<hr>
## Public Functions Documentation




### function AABB [1/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::AABB::AABB (
    const Vector3 & min,
    const Vector3 & max
) 
```




<hr>



### function AABB [2/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::AABB::AABB (
    const AABB & l,
    const AABB & r
) 
```




<hr>



### function center 

```C++
inline MUDA_GENERIC Vector3 muda::spatial_hash::AABB::center () const
```




<hr>



### function radius 

```C++
inline MUDA_GENERIC float muda::spatial_hash::AABB::radius () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/bounding_volume.h`

