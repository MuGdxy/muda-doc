

# Class muda::spatial\_hash::SparseSpatialHash

**template &lt;typename Hash&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**SparseSpatialHash**](classmuda_1_1spatial__hash_1_1_sparse_spatial_hash.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SparseSpatialHash**](#function-sparsespatialhash) ([**muda::Stream**](classmuda_1_1_stream.md) & stream=muda::Stream::Default()) <br> |
|  void | [**detect**](#function-detect-12) ([**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) &gt; spheres, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs, Pred && pred={}) <br>_Detect collision pairs from bounding spheres. Note that:_  |
|  void | [**detect**](#function-detect-22) (int level, [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; [**BoundingSphere**](classmuda_1_1spatial__hash_1_1_bounding_sphere.md) &gt; spheres, [**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) &gt; & collisionPairs, Pred && pred={}) <br>_Detect collision pairs from bounding spheres at a specific level (level &gt;= 0). This is used for hierarchical spatial hashing collision detection. Its user's responsibility to set_ `level` _value to a bounding sphere. Normally, higher level means larger bounding sphere. Users should decide a proper range of radius for each level, like:_ |




























## Public Functions Documentation




### function SparseSpatialHash 

```C++
inline muda::spatial_hash::SparseSpatialHash::SparseSpatialHash (
    muda::Stream & stream=muda::Stream::Default()
) 
```




<hr>



### function detect [1/2]

_Detect collision pairs from bounding spheres. Note that:_ 
```C++
template<typename Pred>
inline void muda::spatial_hash::SparseSpatialHash::detect (
    CBufferView < BoundingSphere > spheres,
    DeviceBuffer < CollisionPair > & collisionPairs,
    Pred && pred={}
) 
```




* The collision pairs are unique but not sorted.
* All `(i,j)` pairs in collisionPairs satisfy `i < j`.






**Parameters:**


* `spheres` bounding spheres 
* `collisionPairs` output collision pairs 
* `pred` predication function. f: `__device__ (int i, int j) -> bool`. If `pred(i,j)` is true, then the collision pair `(i,j)` is recorded, else the collision pair is discarded. 



**See also:** [**DefaultPredication**](classmuda_1_1spatial__hash_1_1_default_predication.md) 



        

<hr>



### function detect [2/2]

_Detect collision pairs from bounding spheres at a specific level (level &gt;= 0). This is used for hierarchical spatial hashing collision detection. Its user's responsibility to set_ `level` _value to a bounding sphere. Normally, higher level means larger bounding sphere. Users should decide a proper range of radius for each level, like:_
```C++
template<typename Pred>
inline void muda::spatial_hash::SparseSpatialHash::detect (
    int level,
    CBufferView < BoundingSphere > spheres,
    DeviceBuffer < CollisionPair > & collisionPairs,
    Pred && pred={}
) 
```




```C++
BoundingSphere s{o,r};
if (r < r0) s.level = 0;
else if (r < r1) s.level = 1;
else s.level = 2;
...
```
 Note that:
* For a level `L`, any bounding spheres has a `level <= L` will be taken into account.
* The collision pairs are unique but not sorted.
* All `(i,j)` pairs in collisionPairs satisfy `i < j`.
* The `collisionPairs` will be appended with new collision pairs (not cleared).




Typical usage: 
```C++
DeviceBuffer<BoundingSphere> spheres;

// Your code to fill spheres with proper level
// ...

DeviceBuffer<CollisionPair> collisionPairs;

for (int level = 0; level < level_count; ++level)
{
    detect(level, spheres, collisionPairs);
}
```





**Parameters:**


* `level` the hierarchy level we want to detect 
* `spheres` bounding spheres 
* `collisionPairs` appended output collision pairs 
* `pred` predication function. f: `__device__ (int i, int j) -> bool`. If `pred(i,j)` is true, then the collision pair `(i,j)` is recorded, else the collision pair is discarded.



**See also:** [**DefaultPredication**](classmuda_1_1spatial__hash_1_1_default_predication.md) 



        

<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/sparse_spatial_hash.h`

