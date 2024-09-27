

# Class muda::spatial\_hash::SpatialHashTableInfo

**template &lt;typename Hash&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**SpatialHashTableInfo**](classmuda_1_1spatial__hash_1_1_spatial_hash_table_info.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  Float | [**cell\_size**](#variable-cell_size)   = = 0.0f<br> |
|  Vector3 | [**coord\_min**](#variable-coord_min)   = = Vector3::Zero()<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**SpatialHashTableInfo**](#function-spatialhashtableinfo-12) () = default<br> |
|  MUDA\_GENERIC | [**SpatialHashTableInfo**](#function-spatialhashtableinfo-22) (Float cell\_size, const Vector3 & coord\_min) <br> |
|  MUDA\_GENERIC Vector3u | [**cell**](#function-cell) (const Vector3 & xyz) const<br> |
|  MUDA\_GENERIC Vector3 | [**cell\_center\_coord**](#function-cell_center_coord) (const Vector3u & ijk) const<br> |
|  MUDA\_GENERIC Vector3 | [**coord**](#function-coord) (const Vector3u & ijk) const<br> |
|  MUDA\_GENERIC U32 | [**hash\_cell**](#function-hash_cell-12) (const Vector3 & xyz) const<br> |
|  MUDA\_GENERIC U32 | [**hash\_cell**](#function-hash_cell-22) (const Vector3u & ijk) const<br> |




























## Public Attributes Documentation




### variable cell\_size 

```C++
Float muda::spatial_hash::SpatialHashTableInfo< Hash >::cell_size;
```




<hr>



### variable coord\_min 

```C++
Vector3 muda::spatial_hash::SpatialHashTableInfo< Hash >::coord_min;
```




<hr>
## Public Functions Documentation




### function SpatialHashTableInfo [1/2]

```C++
MUDA_GENERIC muda::spatial_hash::SpatialHashTableInfo::SpatialHashTableInfo () = default
```




<hr>



### function SpatialHashTableInfo [2/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::SpatialHashTableInfo::SpatialHashTableInfo (
    Float cell_size,
    const Vector3 & coord_min
) 
```




<hr>



### function cell 

```C++
inline MUDA_GENERIC Vector3u muda::spatial_hash::SpatialHashTableInfo::cell (
    const Vector3 & xyz
) const
```




<hr>



### function cell\_center\_coord 

```C++
inline MUDA_GENERIC Vector3 muda::spatial_hash::SpatialHashTableInfo::cell_center_coord (
    const Vector3u & ijk
) const
```




<hr>



### function coord 

```C++
inline MUDA_GENERIC Vector3 muda::spatial_hash::SpatialHashTableInfo::coord (
    const Vector3u & ijk
) const
```




<hr>



### function hash\_cell [1/2]

```C++
inline MUDA_GENERIC U32 muda::spatial_hash::SpatialHashTableInfo::hash_cell (
    const Vector3 & xyz
) const
```




<hr>



### function hash\_cell [2/2]

```C++
inline MUDA_GENERIC U32 muda::spatial_hash::SpatialHashTableInfo::hash_cell (
    const Vector3u & ijk
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/sparse_spatial_hash_impl.h`

