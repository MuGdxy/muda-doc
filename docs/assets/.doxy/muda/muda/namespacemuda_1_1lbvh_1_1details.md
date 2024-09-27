

# Namespace muda::lbvh::details



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**details**](namespacemuda_1_1lbvh_1_1details.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md) &lt;IsConst, typename Real, typename Object&gt;<br> |
| struct | [**Node**](structmuda_1_1lbvh_1_1details_1_1_node.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**construct\_internal\_nodes**](#function-construct_internal_nodes) (const thrust::detail::execution\_policy\_base&lt; DerivedPolicy &gt; & policy, [**Node**](structmuda_1_1lbvh_1_1details_1_1_node.md) \* nodes, UInt const \* node\_code, const uint32\_t num\_objects) <br> |
|  MUDA\_GENERIC uint2 | [**determine\_range**](#function-determine_range) (UInt const \* node\_code, const uint32\_t num\_leaves, uint32\_t idx) <br> |
|  MUDA\_GENERIC uint32\_t | [**find\_split**](#function-find_split) (UInt const \* node\_code, const uint32\_t num\_leaves, const uint32\_t first, const uint32\_t last) noexcept<br> |




























## Public Functions Documentation




### function construct\_internal\_nodes 

```C++
template<typename DerivedPolicy, typename UInt>
void muda::lbvh::details::construct_internal_nodes (
    const thrust::detail::execution_policy_base< DerivedPolicy > & policy,
    Node * nodes,
    UInt const * node_code,
    const uint32_t num_objects
) 
```




<hr>



### function determine\_range 

```C++
template<typename UInt>
MUDA_GENERIC uint2 muda::lbvh::details::determine_range (
    UInt const * node_code,
    const uint32_t num_leaves,
    uint32_t idx
) 
```




<hr>



### function find\_split 

```C++
template<typename UInt>
MUDA_GENERIC uint32_t muda::lbvh::details::find_split (
    UInt const * node_code,
    const uint32_t num_leaves,
    const uint32_t first,
    const uint32_t last
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/bvh.h`

