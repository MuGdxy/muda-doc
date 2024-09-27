

# Struct muda::lbvh::AABB

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md)&lt; T &gt;::type | [**lower**](#variable-lower)  <br> |
|  [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md)&lt; T &gt;::type | [**upper**](#variable-upper)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**AABB**](#function-aabb-13) () noexcept<br> |
|  MUDA\_GENERIC | [**AABB**](#function-aabb-23) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; &) noexcept<br> |
|  MUDA\_GENERIC | [**AABB**](#function-aabb-33) ([**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; &&) noexcept<br> |
|  MUDA\_GENERIC [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md) & | [**operator=**](#function-operator) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; &) noexcept<br> |
|  MUDA\_GENERIC [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md) & | [**operator=**](#function-operator_1) ([**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; &&) noexcept<br> |




























## Public Attributes Documentation




### variable lower 

```C++
vector_of<T>::type muda::lbvh::AABB< T >::lower;
```




<hr>



### variable upper 

```C++
vector_of<T>::type muda::lbvh::AABB< T >::upper;
```




<hr>
## Public Functions Documentation




### function AABB [1/3]

```C++
MUDA_GENERIC muda::lbvh::AABB::AABB () noexcept
```




<hr>



### function AABB [2/3]

```C++
MUDA_GENERIC muda::lbvh::AABB::AABB (
    const AABB < T > &
) noexcept
```




<hr>



### function AABB [3/3]

```C++
MUDA_GENERIC muda::lbvh::AABB::AABB (
    AABB < T > &&
) noexcept
```




<hr>



### function operator= 

```C++
MUDA_GENERIC AABB & muda::lbvh::AABB::operator= (
    const AABB < T > &
) noexcept
```




<hr>



### function operator= 

```C++
MUDA_GENERIC AABB & muda::lbvh::AABB::operator= (
    AABB < T > &&
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/aabb.h`

