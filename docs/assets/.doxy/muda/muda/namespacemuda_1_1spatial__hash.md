

# Namespace muda::spatial\_hash



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**details**](namespacemuda_1_1spatial__hash_1_1details.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) <br> |
| class | [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) <br> |
| class | [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) <br> |
| class | [**DefaultPredication**](classmuda_1_1spatial__hash_1_1_default_predication.md) <br> |
| class | [**Morton**](classmuda_1_1spatial__hash_1_1_morton.md) &lt;typename T&gt;<br> |
| class | [**Morton&lt; uint32\_t &gt;**](classmuda_1_1spatial__hash_1_1_morton_3_01uint32__t_01_4.md) &lt;&gt;<br> |
| class | [**Morton&lt; uint64\_t &gt;**](classmuda_1_1spatial__hash_1_1_morton_3_01uint64__t_01_4.md) &lt;&gt;<br> |
| class | [**SparseSpatialHash**](classmuda_1_1spatial__hash_1_1_sparse_spatial_hash.md) &lt;typename Hash&gt;<br> |
| class | [**SpatialHashTableInfo**](classmuda_1_1spatial__hash_1_1_spatial_hash_table_info.md) &lt;typename Hash&gt;<br> |
| class | [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) <br>_To represent a cell-object pair in the spatial hash 3D grid e.g. (cell\_id,object\_id) = (1024, 32) for the meaning: the 32th object overlap with the 1024th cell._  |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_GENERIC float | [**distance**](#function-distance) (const Eigen::Vector3f & p, [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) b) <br> |
|  MUDA\_INLINE MUDA\_GENERIC bool | [**intersect**](#function-intersect) (const [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) & s, const [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) & b) <br> |
|  MUDA\_INLINE MUDA\_GENERIC bool | [**intersect**](#function-intersect) (const [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) & lhs, const [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) & rhs) <br> |
|  MUDA\_INLINE MUDA\_GENERIC bool | [**intersect**](#function-intersect) (const [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) & l, const [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) & r) <br> |
|  MUDA\_INLINE MUDA\_GENERIC float | [**squared\_distance**](#function-squared_distance) (const Eigen::Vector3f & p, [**AABB**](classmuda_1_1spatial__hash_1_1_a_a_b_b.md) b) <br> |




























## Public Functions Documentation




### function distance 

```C++
MUDA_INLINE MUDA_GENERIC float muda::spatial_hash::distance (
    const Eigen::Vector3f & p,
    AABB b
) 
```




<hr>



### function intersect 

```C++
MUDA_INLINE MUDA_GENERIC bool muda::spatial_hash::intersect (
    const BoundingSphere & s,
    const AABB & b
) 
```




<hr>



### function intersect 

```C++
MUDA_INLINE MUDA_GENERIC bool muda::spatial_hash::intersect (
    const BoundingSphere & lhs,
    const BoundingSphere & rhs
) 
```




<hr>



### function intersect 

```C++
MUDA_INLINE MUDA_GENERIC bool muda::spatial_hash::intersect (
    const AABB & l,
    const AABB & r
) 
```




<hr>



### function squared\_distance 

```C++
MUDA_INLINE MUDA_GENERIC float muda::spatial_hash::squared_distance (
    const Eigen::Vector3f & p,
    AABB b
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/bounding_volume.h`

