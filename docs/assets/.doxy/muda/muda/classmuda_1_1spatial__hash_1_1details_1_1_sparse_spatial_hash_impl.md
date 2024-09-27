

# Class muda::spatial\_hash::details::SparseSpatialHashImpl

**template &lt;typename Hash&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**details**](namespacemuda_1_1spatial__hash_1_1details.md) **>** [**SparseSpatialHashImpl**](classmuda_1_1spatial__hash_1_1details_1_1_sparse_spatial_hash_impl.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) | [**Cell**](#typedef-cell)  <br> |
| typedef int32\_t | [**I32**](#typedef-i32)  <br> |
| typedef uint32\_t | [**U32**](#typedef-u32)  <br> |
| typedef Eigen::Vector3f | [**Vector3**](#typedef-vector3)  <br> |
| typedef Eigen::Vector3&lt; I32 &gt; | [**Vector3i**](#typedef-vector3i)  <br> |
| typedef Eigen::Vector3&lt; U32 &gt; | [**Vector3u**](#typedef-vector3u)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; Vector3 &gt; | [**allCoords**](#variable-allcoords)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; float &gt; | [**allRadius**](#variable-allradius)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**cellArrayKey**](#variable-cellarraykey)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**cellArrayKeySorted**](#variable-cellarraykeysorted)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) &gt; | [**cellArrayValue**](#variable-cellarrayvalue)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) &gt; | [**cellArrayValueSorted**](#variable-cellarrayvaluesorted)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; int &gt; | [**cellCount**](#variable-cellcount)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**cellToCollisionPairUpperBound**](#variable-celltocollisionpairupperbound)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**cellToCollisionPairUpperBoundPrefixSum**](#variable-celltocollisionpairupperboundprefixsum)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; | [**collisionPairBuffer**](#variable-collisionpairbuffer)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**collisionPairCount**](#variable-collisionpaircount)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**collisionPairPrefixSum**](#variable-collisionpairprefixsum)  <br> |
|  bool | [**empty\_level**](#variable-empty_level)   = = false<br> |
|  [**SpatialHashTableInfo**](classmuda_1_1spatial__hash_1_1_spatial_hash_table_info.md)&lt; Hash &gt; | [**h\_spatialHashConfig**](#variable-h_spatialhashconfig)  <br> |
|  int | [**level**](#variable-level)   = = 0<br> |
|  [**muda::Stream**](classmuda_1_1_stream.md) & | [**m\_stream**](#variable-m_stream)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; float &gt; | [**maxRadius**](#variable-maxradius)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; Vector3 &gt; | [**minCoord**](#variable-mincoord)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**objCountInCell**](#variable-objcountincell)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**objCountInCellPrefixSum**](#variable-objcountincellprefixsum)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; int &gt; | [**pairCount**](#variable-paircount)  <br> |
|  size\_t | [**pairListOffset**](#variable-pairlistoffset)   = = 0<br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**potentialCollisionPairIdToCellIndex**](#variable-potentialcollisionpairidtocellindex)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**potentialCollisionPairIdToCellIndexBuffer**](#variable-potentialcollisionpairidtocellindexbuffer)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; [**SpatialHashTableInfo**](classmuda_1_1spatial__hash_1_1_spatial_hash_table_info.md)&lt; Hash &gt; &gt; | [**spatialHashConfig**](#variable-spatialhashconfig)  <br> |
|  [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) &gt; | [**spheres**](#variable-spheres)  <br> |
|  int | [**sum**](#variable-sum)  <br> |
|  [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; int &gt; | [**uniqueKey**](#variable-uniquekey)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; int &gt; | [**uniqueKeyCount**](#variable-uniquekeycount)  <br> |
|  int | [**validCellCount**](#variable-validcellcount)  <br> |
|  [**DeviceVar**](classmuda_1_1_device_var.md)&lt; int &gt; | [**validCollisionPairCount**](#variable-validcollisionpaircount)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SparseSpatialHashImpl**](#function-sparsespatialhashimpl) ([**muda::Stream**](classmuda_1_1_stream.md) & stream=muda::Stream::Default()) <br> |
|  void | [**alloc\_collision\_pair\_list**](#function-alloc_collision_pair_list) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs, int totalCollisionPairCount) <br> |
|  void | [**balanced\_setup\_collision\_pairs**](#function-balanced_setup_collision_pairs) (bool append, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs, Pred && pred) <br> |
|  void | [**calculate\_hash\_table\_basic\_info**](#function-calculate_hash_table_basic_info) () <br> |
|  void | [**count\_object\_per\_cell**](#function-count_object_per_cell) () <br> |
|  void | [**detect**](#function-detect) ([**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) &gt; boundingSphereList, bool append, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs, Pred && pred) <br> |
|  void | [**fill\_hash\_cells**](#function-fill_hash_cells) () <br> |
|  void | [**setup\_hash\_table**](#function-setup_hash_table) () <br> |
|  void | [**simple\_count\_collision\_pairs**](#function-simple_count_collision_pairs) (Pred && pred) <br> |
|  void | [**simple\_fill\_collision\_pair\_list**](#function-simple_fill_collision_pair_list) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs, Pred && pred) <br> |
|  void | [**simple\_setup\_collision\_pairs**](#function-simple_setup_collision_pairs) (Pred && pred, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs) <br> |




























## Public Types Documentation




### typedef Cell 

```C++
using muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::Cell =  SpatialPartitionCell;
```




<hr>



### typedef I32 

```C++
using muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::I32 =  int32_t;
```




<hr>



### typedef U32 

```C++
using muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::U32 =  uint32_t;
```




<hr>



### typedef Vector3 

```C++
using muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::Vector3 =  Eigen::Vector3f;
```




<hr>



### typedef Vector3i 

```C++
using muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::Vector3i =  Eigen::Vector3<I32>;
```




<hr>



### typedef Vector3u 

```C++
using muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::Vector3u =  Eigen::Vector3<U32>;
```




<hr>
## Public Attributes Documentation




### variable allCoords 

```C++
DeviceBuffer<Vector3> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::allCoords;
```




<hr>



### variable allRadius 

```C++
DeviceBuffer<float> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::allRadius;
```




<hr>



### variable cellArrayKey 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellArrayKey;
```




<hr>



### variable cellArrayKeySorted 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellArrayKeySorted;
```




<hr>



### variable cellArrayValue 

```C++
DeviceBuffer<SpatialPartitionCell> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellArrayValue;
```




<hr>



### variable cellArrayValueSorted 

```C++
DeviceBuffer<SpatialPartitionCell> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellArrayValueSorted;
```




<hr>



### variable cellCount 

```C++
DeviceVar<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellCount;
```




<hr>



### variable cellToCollisionPairUpperBound 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellToCollisionPairUpperBound;
```




<hr>



### variable cellToCollisionPairUpperBoundPrefixSum 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::cellToCollisionPairUpperBoundPrefixSum;
```




<hr>



### variable collisionPairBuffer 

```C++
DeviceBuffer<CollisionPair> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::collisionPairBuffer;
```




<hr>



### variable collisionPairCount 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::collisionPairCount;
```




<hr>



### variable collisionPairPrefixSum 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::collisionPairPrefixSum;
```




<hr>



### variable empty\_level 

```C++
bool muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::empty_level;
```




<hr>



### variable h\_spatialHashConfig 

```C++
SpatialHashTableInfo<Hash> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::h_spatialHashConfig;
```




<hr>



### variable level 

```C++
int muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::level;
```




<hr>



### variable m\_stream 

```C++
muda::Stream& muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::m_stream;
```




<hr>



### variable maxRadius 

```C++
DeviceVar<float> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::maxRadius;
```




<hr>



### variable minCoord 

```C++
DeviceVar<Vector3> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::minCoord;
```




<hr>



### variable objCountInCell 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::objCountInCell;
```




<hr>



### variable objCountInCellPrefixSum 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::objCountInCellPrefixSum;
```




<hr>



### variable pairCount 

```C++
DeviceVar<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::pairCount;
```




<hr>



### variable pairListOffset 

```C++
size_t muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::pairListOffset;
```




<hr>



### variable potentialCollisionPairIdToCellIndex 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::potentialCollisionPairIdToCellIndex;
```




<hr>



### variable potentialCollisionPairIdToCellIndexBuffer 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::potentialCollisionPairIdToCellIndexBuffer;
```




<hr>



### variable spatialHashConfig 

```C++
DeviceVar<SpatialHashTableInfo<Hash> > muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::spatialHashConfig;
```




<hr>



### variable spheres 

```C++
CBufferView<BoundingSphere> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::spheres;
```




<hr>



### variable sum 

```C++
int muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::sum;
```




<hr>



### variable uniqueKey 

```C++
DeviceBuffer<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::uniqueKey;
```




<hr>



### variable uniqueKeyCount 

```C++
DeviceVar<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::uniqueKeyCount;
```




<hr>



### variable validCellCount 

```C++
int muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::validCellCount;
```




<hr>



### variable validCollisionPairCount 

```C++
DeviceVar<int> muda::spatial_hash::details::SparseSpatialHashImpl< Hash >::validCollisionPairCount;
```




<hr>
## Public Functions Documentation




### function SparseSpatialHashImpl 

```C++
inline muda::spatial_hash::details::SparseSpatialHashImpl::SparseSpatialHashImpl (
    muda::Stream & stream=muda::Stream::Default()
) 
```




<hr>



### function alloc\_collision\_pair\_list 

```C++
void muda::spatial_hash::details::SparseSpatialHashImpl::alloc_collision_pair_list (
    DeviceBuffer < CollisionPair > & collisionPairs,
    int totalCollisionPairCount
) 
```




<hr>



### function balanced\_setup\_collision\_pairs 

```C++
template<typename Pred>
void muda::spatial_hash::details::SparseSpatialHashImpl::balanced_setup_collision_pairs (
    bool append,
    DeviceBuffer < CollisionPair > & collisionPairs,
    Pred && pred
) 
```




<hr>



### function calculate\_hash\_table\_basic\_info 

```C++
void muda::spatial_hash::details::SparseSpatialHashImpl::calculate_hash_table_basic_info () 
```




<hr>



### function count\_object\_per\_cell 

```C++
void muda::spatial_hash::details::SparseSpatialHashImpl::count_object_per_cell () 
```




<hr>



### function detect 

```C++
template<typename Pred>
void muda::spatial_hash::details::SparseSpatialHashImpl::detect (
    CBufferView < BoundingSphere > boundingSphereList,
    bool append,
    DeviceBuffer < CollisionPair > & collisionPairs,
    Pred && pred
) 
```




<hr>



### function fill\_hash\_cells 

```C++
void muda::spatial_hash::details::SparseSpatialHashImpl::fill_hash_cells () 
```




<hr>



### function setup\_hash\_table 

```C++
void muda::spatial_hash::details::SparseSpatialHashImpl::setup_hash_table () 
```




<hr>



### function simple\_count\_collision\_pairs 

```C++
template<typename Pred>
void muda::spatial_hash::details::SparseSpatialHashImpl::simple_count_collision_pairs (
    Pred && pred
) 
```




<hr>



### function simple\_fill\_collision\_pair\_list 

```C++
template<typename Pred>
void muda::spatial_hash::details::SparseSpatialHashImpl::simple_fill_collision_pair_list (
    DeviceBuffer < CollisionPair > & collisionPairs,
    Pred && pred
) 
```




<hr>



### function simple\_setup\_collision\_pairs 

```C++
template<typename Pred>
void muda::spatial_hash::details::SparseSpatialHashImpl::simple_setup_collision_pairs (
    Pred && pred,
    DeviceBuffer < CollisionPair > & collisionPairs
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/sparse_spatial_hash_impl.h`

