

# Class muda::spatial\_hash::SpatialPartitionCell



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md)



_To represent a cell-object pair in the spatial hash 3D grid e.g. (cell\_id,object\_id) = (1024, 32) for the meaning: the 32th object overlap with the 1024th cell._ 

* `#include <sparse_spatial_hash_impl.h>`

















## Public Types

| Type | Name |
| ---: | :--- |
| typedef uint32\_t | [**U32**](#typedef-u32)  <br> |
| typedef Eigen::Vector3&lt; uint32\_t &gt; | [**Vector3u**](#typedef-vector3u)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  U32 | [**cid**](#variable-cid)  <br> |
|  struct [**muda::spatial\_hash::SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) | [**ctlbit**](#variable-ctlbit)  <br> |
|  U32 | [**home**](#variable-home)  <br> |
|  U32 | [**oid**](#variable-oid)  <br> |
|  U32 | [**overlap**](#variable-overlap)  <br> |
|  U32 | [**pass**](#variable-pass)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**SpatialPartitionCell**](#function-spatialpartitioncell-12) () <br> |
|  MUDA\_GENERIC | [**SpatialPartitionCell**](#function-spatialpartitioncell-22) (U32 cid, U32 oid) <br> |
|  MUDA\_GENERIC bool | [**is\_home**](#function-is_home) () const<br> |
|  MUDA\_GENERIC bool | [**is\_phantom**](#function-is_phantom) () const<br> |
|  MUDA\_GENERIC void | [**set\_as\_home**](#function-set_as_home) (const Vector3u & ijk) <br> |
|  MUDA\_GENERIC void | [**set\_as\_phantom**](#function-set_as_phantom) (const Vector3u & home\_ijk, const Vector3u & cell\_ijk) <br> |
|  MUDA\_GENERIC void | [**set\_overlap**](#function-set_overlap) (const Vector3u & ijk) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC bool | [**allow\_ignore**](#function-allow_ignore) (const [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) & l, const [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) & r) <br> |
|  MUDA\_GENERIC U32 | [**pass\_type**](#function-pass_type) (const Vector3u & ijk) <br> |


























## Public Types Documentation




### typedef U32 

```C++
using muda::spatial_hash::SpatialPartitionCell::U32 =  uint32_t;
```




<hr>



### typedef Vector3u 

```C++
using muda::spatial_hash::SpatialPartitionCell::Vector3u =  Eigen::Vector3<uint32_t>;
```




<hr>
## Public Attributes Documentation




### variable cid 

```C++
U32 muda::spatial_hash::SpatialPartitionCell::cid;
```




<hr>



### variable ctlbit 

```C++
struct muda::spatial_hash::SpatialPartitionCell muda::spatial_hash::SpatialPartitionCell::ctlbit;
```




<hr>



### variable home 

```C++
U32 muda::spatial_hash::SpatialPartitionCell::home;
```




<hr>



### variable oid 

```C++
U32 muda::spatial_hash::SpatialPartitionCell::oid;
```




<hr>



### variable overlap 

```C++
U32 muda::spatial_hash::SpatialPartitionCell::overlap;
```




<hr>



### variable pass 

```C++
U32 muda::spatial_hash::SpatialPartitionCell::pass;
```




<hr>
## Public Functions Documentation




### function SpatialPartitionCell [1/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::SpatialPartitionCell::SpatialPartitionCell () 
```




<hr>



### function SpatialPartitionCell [2/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::SpatialPartitionCell::SpatialPartitionCell (
    U32 cid,
    U32 oid
) 
```




<hr>



### function is\_home 

```C++
inline MUDA_GENERIC bool muda::spatial_hash::SpatialPartitionCell::is_home () const
```




<hr>



### function is\_phantom 

```C++
inline MUDA_GENERIC bool muda::spatial_hash::SpatialPartitionCell::is_phantom () const
```




<hr>



### function set\_as\_home 

```C++
inline MUDA_GENERIC void muda::spatial_hash::SpatialPartitionCell::set_as_home (
    const Vector3u & ijk
) 
```




<hr>



### function set\_as\_phantom 

```C++
inline MUDA_GENERIC void muda::spatial_hash::SpatialPartitionCell::set_as_phantom (
    const Vector3u & home_ijk,
    const Vector3u & cell_ijk
) 
```




<hr>



### function set\_overlap 

```C++
inline MUDA_GENERIC void muda::spatial_hash::SpatialPartitionCell::set_overlap (
    const Vector3u & ijk
) 
```




<hr>
## Public Static Functions Documentation




### function allow\_ignore 

```C++
static inline MUDA_GENERIC bool muda::spatial_hash::SpatialPartitionCell::allow_ignore (
    const SpatialPartitionCell & l,
    const SpatialPartitionCell & r
) 
```




<hr>



### function pass\_type 

```C++
static inline MUDA_GENERIC U32 muda::spatial_hash::SpatialPartitionCell::pass_type (
    const Vector3u & ijk
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/sparse_spatial_hash_impl.h`

