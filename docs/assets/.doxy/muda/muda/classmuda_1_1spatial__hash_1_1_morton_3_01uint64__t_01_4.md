

# Class muda::spatial\_hash::Morton&lt; uint64\_t &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**Morton&lt; uint64\_t &gt;**](classmuda_1_1spatial__hash_1_1_morton_3_01uint64__t_01_4.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Vector3&lt; uint32\_t &gt; | [**Vector3u**](#typedef-vector3u)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC uint64\_t | [**operator()**](#function-operator()-12) (const Vector3u & p) const<br> |
|  constexpr MUDA\_GENERIC uint64\_t | [**operator()**](#function-operator()-22) (uint32\_t x, uint32\_t y, uint32\_t z) const<br> |




























## Public Types Documentation




### typedef Vector3u 

```C++
using muda::spatial_hash::Morton< uint64_t >::Vector3u =  Eigen::Vector3<uint32_t>;
```




<hr>
## Public Functions Documentation




### function operator() [1/2]

```C++
inline MUDA_GENERIC uint64_t muda::spatial_hash::Morton< uint64_t >::operator() (
    const Vector3u & p
) const
```




<hr>



### function operator() [2/2]

```C++
inline constexpr MUDA_GENERIC uint64_t muda::spatial_hash::Morton< uint64_t >::operator() (
    uint32_t x,
    uint32_t y,
    uint32_t z
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/morton_hash.h`

