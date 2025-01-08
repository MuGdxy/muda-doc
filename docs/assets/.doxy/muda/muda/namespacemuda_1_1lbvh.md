

# Namespace muda::lbvh



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**details**](namespacemuda_1_1lbvh_1_1details.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md) &lt;typename T&gt;<br> |
| class | [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md) &lt;typename Real, typename Object, typename AABBGetter, typename MortonCodeCalculator&gt;<br> |
| struct | [**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) &lt;typename Real, typename Object&gt;<br> |
| struct | [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md) &lt;typename Real&gt;<br> |
| struct | [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md) &lt;typename Real&gt;<br> |
| struct | [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md) &lt;typename T&gt;<br> |
| struct | [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md) &lt;typename T&gt;<br> |
| struct | [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md) &lt;typename T&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**details::BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; false, Real, Object &gt; | [**BVHViewer**](#typedef-bvhviewer)  <br> |
| typedef [**details::BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; true, Real, Object &gt; | [**CBVHViewer**](#typedef-cbvhviewer)  <br> |
| typedef typename [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md)&lt; T &gt;::type | [**vector\_of\_t**](#typedef-vector_of_t)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC [**vector\_of**](structmuda_1_1lbvh_1_1vector__of.md)&lt; T &gt;::type | [**centroid**](#function-centroid) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; & box) noexcept<br> |
|  \_\_device\_\_ MUDA\_INLINE int | [**common\_upper\_bits**](#function-common_upper_bits) (const unsigned int lhs, const unsigned int rhs) noexcept<br> |
|  \_\_device\_\_ MUDA\_INLINE int | [**common\_upper\_bits**](#function-common_upper_bits) (const unsigned long long int lhs, const unsigned long long int rhs) noexcept<br> |
|  MUDA\_GENERIC MUDA\_INLINE std::uint32\_t | [**expand\_bits**](#function-expand_bits) (std::uint32\_t v) noexcept<br> |
|  \_\_device\_\_ T | [**infinity**](#function-infinity) () noexcept<br> |
|  \_\_device\_\_ double | [**infinity&lt; double &gt;**](#function-infinity<-double->) () noexcept<br> |
|  \_\_device\_\_ float | [**infinity&lt; float &gt;**](#function-infinity<-float->) () noexcept<br> |
|  MUDA\_GENERIC bool | [**intersects**](#function-intersects) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; & lhs, const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; T &gt; & rhs) noexcept<br> |
|  MUDA\_GENERIC [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; double &gt; | [**merge**](#function-merge) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; double &gt; & lhs, const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; double &gt; & rhs) noexcept<br> |
|  MUDA\_GENERIC [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; float &gt; | [**merge**](#function-merge) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; float &gt; & lhs, const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; float &gt; & rhs) noexcept<br> |
|  MUDA\_GENERIC float | [**mindist**](#function-mindist) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; float &gt; & lhs, const float4 & rhs) noexcept<br> |
|  MUDA\_GENERIC double | [**mindist**](#function-mindist) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; double &gt; & lhs, const double4 & rhs) noexcept<br> |
|  MUDA\_GENERIC float | [**minmaxdist**](#function-minmaxdist) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; float &gt; & lhs, const float4 & rhs) noexcept<br> |
|  MUDA\_GENERIC double | [**minmaxdist**](#function-minmaxdist) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; double &gt; & lhs, const double4 & rhs) noexcept<br> |
|  MUDA\_GENERIC MUDA\_INLINE std::uint32\_t | [**morton\_code**](#function-morton_code) (float4 xyz, float resolution=1024.0f) noexcept<br> |
|  MUDA\_GENERIC MUDA\_INLINE std::uint32\_t | [**morton\_code**](#function-morton_code) (double4 xyz, double resolution=1024.0) noexcept<br> |
|  MUDA\_GENERIC [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)&lt; float &gt; | [**nearest**](#function-nearest) (const float4 & point) noexcept<br> |
|  MUDA\_GENERIC [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)&lt; float &gt; | [**nearest**](#function-nearest) (const float3 & point) noexcept<br> |
|  MUDA\_GENERIC [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)&lt; double &gt; | [**nearest**](#function-nearest) (const double4 & point) noexcept<br> |
|  MUDA\_GENERIC [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)&lt; double &gt; | [**nearest**](#function-nearest) (const double3 & point) noexcept<br> |
|  MUDA\_GENERIC [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md)&lt; Real &gt; | [**overlaps**](#function-overlaps) (const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; & region) noexcept<br> |
|  MUDA\_HOST uint32\_t | [**query**](#function-query) (const [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md)&lt; Real, Objects, AABBGetter, MortonCodeCalculator &gt; & tree, const [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md)&lt; Real &gt; q, OutputBackInserter outiter) noexcept<br> |
|  MUDA\_HOST std::pair&lt; uint32\_t, Real &gt; | [**query**](#function-query) (const [**BVH**](classmuda_1_1lbvh_1_1_b_v_h.md)&lt; Real, Objects, AABBGetter, MortonCodeCalculator &gt; & tree, const [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)&lt; Real &gt; & q, DistanceCalculator calc\_dist) noexcept<br> |




























## Public Types Documentation




### typedef BVHViewer 

```C++
using muda::lbvh::BVHViewer =  details::BVHViewerBase<false, Real, Object>;
```




<hr>



### typedef CBVHViewer 

```C++
using muda::lbvh::CBVHViewer =  details::BVHViewerBase<true, Real, Object>;
```




<hr>



### typedef vector\_of\_t 

```C++
using muda::lbvh::vector_of_t =  typename vector_of<T>::type;
```




<hr>
## Public Functions Documentation




### function centroid 

```C++
template<typename T>
inline MUDA_GENERIC vector_of < T >::type muda::lbvh::centroid (
    const AABB < T > & box
) noexcept
```




<hr>



### function common\_upper\_bits 

```C++
__device__ MUDA_INLINE int muda::lbvh::common_upper_bits (
    const unsigned int lhs,
    const unsigned int rhs
) noexcept
```




<hr>



### function common\_upper\_bits 

```C++
__device__ MUDA_INLINE int muda::lbvh::common_upper_bits (
    const unsigned long long int lhs,
    const unsigned long long int rhs
) noexcept
```




<hr>



### function expand\_bits 

```C++
MUDA_GENERIC MUDA_INLINE std::uint32_t muda::lbvh::expand_bits (
    std::uint32_t v
) noexcept
```




<hr>



### function infinity 

```C++
template<typename T>
inline __device__ T muda::lbvh::infinity () noexcept
```




<hr>



### function infinity&lt; double &gt; 

```C++
template<>
inline __device__ double muda::lbvh::infinity< double > () noexcept
```




<hr>



### function infinity&lt; float &gt; 

```C++
template<>
inline __device__ float muda::lbvh::infinity< float > () noexcept
```




<hr>



### function intersects 

```C++
template<typename T>
inline MUDA_GENERIC bool muda::lbvh::intersects (
    const AABB < T > & lhs,
    const AABB < T > & rhs
) noexcept
```




<hr>



### function merge 

```C++
inline MUDA_GENERIC AABB < double > muda::lbvh::merge (
    const AABB < double > & lhs,
    const AABB < double > & rhs
) noexcept
```




<hr>



### function merge 

```C++
inline MUDA_GENERIC AABB < float > muda::lbvh::merge (
    const AABB < float > & lhs,
    const AABB < float > & rhs
) noexcept
```




<hr>



### function mindist 

```C++
inline MUDA_GENERIC float muda::lbvh::mindist (
    const AABB < float > & lhs,
    const float4 & rhs
) noexcept
```




<hr>



### function mindist 

```C++
inline MUDA_GENERIC double muda::lbvh::mindist (
    const AABB < double > & lhs,
    const double4 & rhs
) noexcept
```




<hr>



### function minmaxdist 

```C++
inline MUDA_GENERIC float muda::lbvh::minmaxdist (
    const AABB < float > & lhs,
    const float4 & rhs
) noexcept
```




<hr>



### function minmaxdist 

```C++
inline MUDA_GENERIC double muda::lbvh::minmaxdist (
    const AABB < double > & lhs,
    const double4 & rhs
) noexcept
```




<hr>



### function morton\_code 

```C++
MUDA_GENERIC MUDA_INLINE std::uint32_t muda::lbvh::morton_code (
    float4 xyz,
    float resolution=1024.0f
) noexcept
```




<hr>



### function morton\_code 

```C++
MUDA_GENERIC MUDA_INLINE std::uint32_t muda::lbvh::morton_code (
    double4 xyz,
    double resolution=1024.0
) noexcept
```




<hr>



### function nearest 

```C++
inline MUDA_GENERIC query_nearest < float > muda::lbvh::nearest (
    const float4 & point
) noexcept
```




<hr>



### function nearest 

```C++
inline MUDA_GENERIC query_nearest < float > muda::lbvh::nearest (
    const float3 & point
) noexcept
```




<hr>



### function nearest 

```C++
inline MUDA_GENERIC query_nearest < double > muda::lbvh::nearest (
    const double4 & point
) noexcept
```




<hr>



### function nearest 

```C++
inline MUDA_GENERIC query_nearest < double > muda::lbvh::nearest (
    const double3 & point
) noexcept
```




<hr>



### function overlaps 

```C++
template<typename Real>
MUDA_GENERIC query_overlap < Real > muda::lbvh::overlaps (
    const AABB < Real > & region
) noexcept
```




<hr>



### function query 

```C++
template<typename Real, typename Objects, typename AABBGetter, typename MortonCodeCalculator, typename OutputBackInserter>
MUDA_HOST uint32_t muda::lbvh::query (
    const BVH < Real, Objects, AABBGetter, MortonCodeCalculator > & tree,
    const query_overlap < Real > q,
    OutputBackInserter outiter
) noexcept
```




<hr>



### function query 

```C++
template<typename Real, typename Objects, typename AABBGetter, typename MortonCodeCalculator, typename DistanceCalculator>
MUDA_HOST std::pair< uint32_t, Real > muda::lbvh::query (
    const BVH < Real, Objects, AABBGetter, MortonCodeCalculator > & tree,
    const query_nearest < Real > & q,
    DistanceCalculator calc_dist
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/aabb.h`

