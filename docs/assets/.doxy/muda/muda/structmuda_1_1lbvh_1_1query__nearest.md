

# Struct muda::lbvh::query\_nearest

**template &lt;typename Real&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef typename [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md)&lt; Real &gt;::type | [**vector\_type**](#typedef-vector_type)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  vector\_type | [**target**](#variable-target)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) & | [**operator=**](#function-operator) (const [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) &) = default<br> |
|  [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) & | [**operator=**](#function-operator_1) ([**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) &&) = default<br> |
|  MUDA\_GENERIC | [**query\_nearest**](#function-query_nearest-14) (const vector\_type & tgt) <br> |
|   | [**query\_nearest**](#function-query_nearest-24) () = default<br> |
|   | [**query\_nearest**](#function-query_nearest-34) (const [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) &) = default<br> |
|   | [**query\_nearest**](#function-query_nearest-44) ([**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) &&) = default<br> |
|   | [**~query\_nearest**](#function-query_nearest) () = default<br> |




























## Public Types Documentation




### typedef vector\_type 

```C++
using muda::lbvh::query_nearest< Real >::vector_type =  typename vector_of<Real>::type;
```




<hr>
## Public Attributes Documentation




### variable target 

```C++
vector_type muda::lbvh::query_nearest< Real >::target;
```




<hr>
## Public Functions Documentation




### function operator= 

```C++
query_nearest & muda::lbvh::query_nearest::operator= (
    const query_nearest &
) = default
```




<hr>



### function operator= 

```C++
query_nearest & muda::lbvh::query_nearest::operator= (
    query_nearest &&
) = default
```




<hr>



### function query\_nearest [1/4]

```C++
inline MUDA_GENERIC muda::lbvh::query_nearest::query_nearest (
    const vector_type & tgt
) 
```




<hr>



### function query\_nearest [2/4]

```C++
muda::lbvh::query_nearest::query_nearest () = default
```




<hr>



### function query\_nearest [3/4]

```C++
muda::lbvh::query_nearest::query_nearest (
    const query_nearest &
) = default
```




<hr>



### function query\_nearest [4/4]

```C++
muda::lbvh::query_nearest::query_nearest (
    query_nearest &&
) = default
```




<hr>



### function ~query\_nearest 

```C++
muda::lbvh::query_nearest::~query_nearest () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/predicator.h`

