

# Struct muda::lbvh::query\_overlap

**template &lt;typename Real&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; | [**target**](#variable-target)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC bool | [**operator()**](#function-operator()) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; & box) noexcept<br> |
|  [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) & | [**operator=**](#function-operator) (const [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) &) = default<br> |
|  [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) & | [**operator=**](#function-operator_1) ([**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) &&) = default<br> |
|  MUDA\_GENERIC | [**query\_overlap**](#function-query_overlap-14) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; & tgt) <br> |
|   | [**query\_overlap**](#function-query_overlap-24) () = default<br> |
|   | [**query\_overlap**](#function-query_overlap-34) (const [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) &) = default<br> |
|   | [**query\_overlap**](#function-query_overlap-44) ([**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) &&) = default<br> |
|   | [**~query\_overlap**](#function-query_overlap) () = default<br> |




























## Public Attributes Documentation




### variable target 

```C++
AABB<Real> muda::lbvh::query_overlap< Real >::target;
```




<hr>
## Public Functions Documentation




### function operator() 

```C++
inline MUDA_GENERIC bool muda::lbvh::query_overlap::operator() (
    const AABB < Real > & box
) noexcept
```




<hr>



### function operator= 

```C++
query_overlap & muda::lbvh::query_overlap::operator= (
    const query_overlap &
) = default
```




<hr>



### function operator= 

```C++
query_overlap & muda::lbvh::query_overlap::operator= (
    query_overlap &&
) = default
```




<hr>



### function query\_overlap [1/4]

```C++
inline MUDA_GENERIC muda::lbvh::query_overlap::query_overlap (
    const AABB < Real > & tgt
) 
```




<hr>



### function query\_overlap [2/4]

```C++
muda::lbvh::query_overlap::query_overlap () = default
```




<hr>



### function query\_overlap [3/4]

```C++
muda::lbvh::query_overlap::query_overlap (
    const query_overlap &
) = default
```




<hr>



### function query\_overlap [4/4]

```C++
muda::lbvh::query_overlap::query_overlap (
    query_overlap &&
) = default
```




<hr>



### function ~query\_overlap 

```C++
muda::lbvh::query_overlap::~query_overlap () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/predicator.h`

