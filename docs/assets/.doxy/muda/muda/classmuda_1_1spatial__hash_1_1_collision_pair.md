

# Class muda::spatial\_hash::CollisionPair



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) **>** [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**CollisionPair**](#function-collisionpair-12) (int i, int j) <br> |
|  MUDA\_GENERIC | [**CollisionPair**](#function-collisionpair-22) () <br> |
|  Eigen::Vector2i | [**IDs**](#function-ids) () const<br> |
|  MUDA\_GENERIC bool | [**is\_valid**](#function-is_valid) () const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC [**CollisionPair**](classmuda_1_1spatial__hash_1_1_collision_pair.md) | [**invalid**](#function-invalid) () <br> |


























## Public Functions Documentation




### function CollisionPair [1/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::CollisionPair::CollisionPair (
    int i,
    int j
) 
```




<hr>



### function CollisionPair [2/2]

```C++
inline MUDA_GENERIC muda::spatial_hash::CollisionPair::CollisionPair () 
```




<hr>



### function IDs 

```C++
inline Eigen::Vector2i muda::spatial_hash::CollisionPair::IDs () const
```




<hr>



### function is\_valid 

```C++
inline MUDA_GENERIC bool muda::spatial_hash::CollisionPair::is_valid () const
```




<hr>
## Public Static Functions Documentation




### function invalid 

```C++
static inline MUDA_GENERIC CollisionPair muda::spatial_hash::CollisionPair::invalid () 
```




<hr>## Friends Documentation





### friend operator&lt; 

```C++
inline MUDA_GENERIC friend bool muda::spatial_hash::CollisionPair::operator< (
    const CollisionPair & l,
    const CollisionPair & r
) 
```




<hr>



### friend operator&lt;&lt; 

```C++
inline std::ostream & muda::spatial_hash::CollisionPair::operator<< (
    std::ostream & os,
    const CollisionPair & c
) 
```




<hr>



### friend operator== 

```C++
inline MUDA_GENERIC friend bool muda::spatial_hash::CollisionPair::operator== (
    const CollisionPair & l,
    const CollisionPair & r
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/collision_pair.h`

