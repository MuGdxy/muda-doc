

# Class muda::lbvh::BVH

**template &lt;typename Real, typename Object, typename AABBGetter, typename MortonCodeCalculator&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef AABBGetter | [**aabb\_getter\_type**](#typedef-aabb_getter_type)  <br> |
| typedef [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; real\_type &gt; | [**aabb\_type**](#typedef-aabb_type)  <br> |
| typedef std::uint32\_t | [**index\_type**](#typedef-index_type)  <br> |
| typedef MortonCodeCalculator | [**morton\_code\_calculator\_type**](#typedef-morton_code_calculator_type)  <br> |
| typedef [**details::Node**](structmuda_1_1lbvh_1_1details_1_1_node.md) | [**node\_type**](#typedef-node_type)  <br> |
| typedef Object | [**object\_type**](#typedef-object_type)  <br> |
| typedef Real | [**real\_type**](#typedef-real_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BVH**](#function-bvh-13) () = default<br> |
|   | [**BVH**](#function-bvh-23) (const [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) &) = default<br> |
|   | [**BVH**](#function-bvh-33) ([**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) &&) = default<br> |
|  const auto & | [**aabbs**](#function-aabbs) () noexcept const<br> |
|  void | [**build**](#function-build) (cudaStream\_t stream=nullptr) <br> |
|  void | [**clear**](#function-clear) () <br> |
|  [**CBVHViewer**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; real\_type, object\_type &gt; | [**cviewer**](#function-cviewer) () noexcept const<br> |
|  const auto & | [**host\_aabbs**](#function-host_aabbs) () noexcept const<br> |
|  const auto & | [**host\_nodes**](#function-host_nodes) () noexcept const<br> |
|  const auto & | [**host\_objects**](#function-host_objects) () noexcept const<br> |
|  const auto & | [**nodes**](#function-nodes) () noexcept const<br> |
|  const auto & | [**objects**](#function-objects-12) () noexcept const<br> |
|  auto & | [**objects**](#function-objects-22) () noexcept<br> |
|  [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) & | [**operator=**](#function-operator) (const [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) &) = default<br> |
|  [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) & | [**operator=**](#function-operator_1) ([**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) &&) = default<br> |
|  [**BVHViewer**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; real\_type, object\_type &gt; | [**viewer**](#function-viewer) () noexcept<br> |
|   | [**~BVH**](#function-bvh) () = default<br> |




























## Public Types Documentation




### typedef aabb\_getter\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::aabb_getter_type =  AABBGetter;
```




<hr>



### typedef aabb\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::aabb_type =  AABB<real_type>;
```




<hr>



### typedef index\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::index_type =  std::uint32_t;
```




<hr>



### typedef morton\_code\_calculator\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::morton_code_calculator_type =  MortonCodeCalculator;
```




<hr>



### typedef node\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::node_type =  details::Node;
```




<hr>



### typedef object\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::object_type =  Object;
```




<hr>



### typedef real\_type 

```C++
using muda::lbvh::BVH< Real, Object, AABBGetter, MortonCodeCalculator >::real_type =  Real;
```




<hr>
## Public Functions Documentation




### function BVH [1/3]

```C++
muda::lbvh::BVH::BVH () = default
```




<hr>



### function BVH [2/3]

```C++
muda::lbvh::BVH::BVH (
    const BVH &
) = default
```




<hr>



### function BVH [3/3]

```C++
muda::lbvh::BVH::BVH (
    BVH &&
) = default
```




<hr>



### function aabbs 

```C++
inline const auto & muda::lbvh::BVH::aabbs () noexcept const
```




<hr>



### function build 

```C++
inline void muda::lbvh::BVH::build (
    cudaStream_t stream=nullptr
) 
```




<hr>



### function clear 

```C++
inline void muda::lbvh::BVH::clear () 
```




<hr>



### function cviewer 

```C++
inline CBVHViewer < real_type, object_type > muda::lbvh::BVH::cviewer () noexcept const
```




<hr>



### function host\_aabbs 

```C++
inline const auto & muda::lbvh::BVH::host_aabbs () noexcept const
```




<hr>



### function host\_nodes 

```C++
inline const auto & muda::lbvh::BVH::host_nodes () noexcept const
```




<hr>



### function host\_objects 

```C++
inline const auto & muda::lbvh::BVH::host_objects () noexcept const
```




<hr>



### function nodes 

```C++
inline const auto & muda::lbvh::BVH::nodes () noexcept const
```




<hr>



### function objects [1/2]

```C++
inline const auto & muda::lbvh::BVH::objects () noexcept const
```




<hr>



### function objects [2/2]

```C++
inline auto & muda::lbvh::BVH::objects () noexcept
```




<hr>



### function operator= 

```C++
BVH & muda::lbvh::BVH::operator= (
    const BVH &
) = default
```




<hr>



### function operator= 

```C++
BVH & muda::lbvh::BVH::operator= (
    BVH &&
) = default
```




<hr>



### function viewer 

```C++
inline BVHViewer < real_type, object_type > muda::lbvh::BVH::viewer () noexcept
```




<hr>



### function ~BVH 

```C++
muda::lbvh::BVH::~BVH () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/bvh.h`

