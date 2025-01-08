

# Class muda::lbvh::details::BVHViewerBase

**template &lt;bool IsConst, typename Real, typename Object&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**details**](namespacemuda_1_1lbvh_1_1details.md) **>** [**BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)












## Classes

| Type | Name |
| ---: | :--- |
| struct | [**DefaultQueryCallback**](structmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base_1_1_default_query_callback.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; true, real\_type, object\_type &gt; | [**ConstViewer**](#typedef-constviewer)  <br> |
| typedef [**BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; false, real\_type, object\_type &gt; | [**NonConstViewer**](#typedef-nonconstviewer)  <br> |
| typedef [**BVHViewerBase**](classmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base.md)&lt; IsConst, real\_type, object\_type &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; real\_type &gt; | [**aabb\_type**](#typedef-aabb_type)  <br> |
| typedef std::uint32\_t | [**index\_type**](#typedef-index_type)  <br> |
| typedef [**details::Node**](structmuda_1_1lbvh_1_1details_1_1_node.md) | [**node\_type**](#typedef-node_type)  <br> |
| typedef Object | [**object\_type**](#typedef-object_type)  <br> |
| typedef Real | [**real\_type**](#typedef-real_type)  <br> |














## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**BVHViewerBase**](#function-bvhviewerbase) (const uint32\_t num\_nodes, const uint32\_t num\_objects, auto\_const\_t&lt; [**node\_type**](structmuda_1_1lbvh_1_1details_1_1_node.md) &gt; \* nodes, auto\_const\_t&lt; [**aabb\_type**](structmuda_1_1lbvh_1_1_a_a_b_b.md) &gt; \* aabbs, auto\_const\_t&lt; object\_type &gt; \* objects) <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () noexcept const<br> |
|  MUDA\_GENERIC auto | [**num\_nodes**](#function-num_nodes) () noexcept const<br> |
|  MUDA\_GENERIC auto | [**num\_objects**](#function-num_objects) () noexcept const<br> |
|  MUDA\_GENERIC auto\_const\_t&lt; object\_type &gt; & | [**object**](#function-object-12) (const uint32\_t idx) noexcept<br> |
|  MUDA\_GENERIC const object\_type & | [**object**](#function-object-22) (const uint32\_t idx) noexcept const<br> |
|  MUDA\_GENERIC | [**operator ConstViewer**](#function-operator-constviewer) () noexcept const<br> |
|  MUDA\_GENERIC uint32\_t | [**query**](#function-query-12) (const [**query\_overlap**](structmuda_1_1lbvh_1_1query__overlap.md)&lt; real\_type &gt; & q, F callback=[**DefaultQueryCallback**](structmuda_1_1lbvh_1_1details_1_1_b_v_h_viewer_base_1_1_default_query_callback.md){}) noexcept const<br> |
|  MUDA\_GENERIC thrust::pair&lt; uint32\_t, real\_type &gt; | [**query**](#function-query-22) (const [**query\_nearest**](structmuda_1_1lbvh_1_1query__nearest.md)&lt; real\_type &gt; & q, FDistanceCalculator calc\_dist) noexcept const<br> |


## Public Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-13) () <br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-23) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-33) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**copy\_label**](classmuda_1_1_viewer_base.md#function-copy_label) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) & other) <br> |
|  MUDA\_GENERIC const char \* | [**kernel\_file**](classmuda_1_1_viewer_base.md#function-kernel_file) () const<br> |
|  MUDA\_GENERIC int | [**kernel\_line**](classmuda_1_1_viewer_base.md#function-kernel_line) () const<br> |
|  MUDA\_GENERIC const char \* | [**kernel\_name**](classmuda_1_1_viewer_base.md#function-kernel_name) () const<br> |
|  MUDA\_GENERIC const char \* | [**name**](classmuda_1_1_viewer_base.md#function-name-13) () const<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator_1) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |








## Protected Types inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_viewer_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_viewer_base.md#typedef-non_const_enable_t)  <br> |








































## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Types Documentation




### typedef ConstViewer 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::ConstViewer =  BVHViewerBase<true, real_type, object_type>;
```




<hr>



### typedef NonConstViewer 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::NonConstViewer =  BVHViewerBase<false, real_type, object_type>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::ThisViewer =  BVHViewerBase<IsConst, real_type, object_type>;
```




<hr>



### typedef aabb\_type 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::aabb_type =  AABB<real_type>;
```




<hr>



### typedef index\_type 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::index_type =  std::uint32_t;
```




<hr>



### typedef node\_type 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::node_type =  details::Node;
```




<hr>



### typedef object\_type 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::object_type =  Object;
```




<hr>



### typedef real\_type 

```C++
using muda::lbvh::details::BVHViewerBase< IsConst, Real, Object >::real_type =  Real;
```




<hr>
## Public Functions Documentation




### function BVHViewerBase 

```C++
inline MUDA_GENERIC muda::lbvh::details::BVHViewerBase::BVHViewerBase (
    const uint32_t num_nodes,
    const uint32_t num_objects,
    auto_const_t< node_type > * nodes,
    auto_const_t< aabb_type > * aabbs,
    auto_const_t< object_type > * objects
) 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::lbvh::details::BVHViewerBase::as_const () noexcept const
```




<hr>



### function num\_nodes 

```C++
inline MUDA_GENERIC auto muda::lbvh::details::BVHViewerBase::num_nodes () noexcept const
```




<hr>



### function num\_objects 

```C++
inline MUDA_GENERIC auto muda::lbvh::details::BVHViewerBase::num_objects () noexcept const
```




<hr>



### function object [1/2]

```C++
inline MUDA_GENERIC auto_const_t< object_type > & muda::lbvh::details::BVHViewerBase::object (
    const uint32_t idx
) noexcept
```




<hr>



### function object [2/2]

```C++
inline MUDA_GENERIC const object_type & muda::lbvh::details::BVHViewerBase::object (
    const uint32_t idx
) noexcept const
```




<hr>



### function operator ConstViewer 

```C++
inline MUDA_GENERIC muda::lbvh::details::BVHViewerBase::operator ConstViewer () noexcept const
```




<hr>



### function query [1/2]

```C++
template<typename F, uint32_t StackNum>
inline MUDA_GENERIC uint32_t muda::lbvh::details::BVHViewerBase::query (
    const query_overlap < real_type > & q,
    F callback=DefaultQueryCallback {}
) noexcept const
```




<hr>



### function query [2/2]

```C++
template<typename FDistanceCalculator, uint32_t StackNum>
inline MUDA_GENERIC thrust::pair< uint32_t, real_type > muda::lbvh::details::BVHViewerBase::query (
    const query_nearest < real_type > & q,
    FDistanceCalculator calc_dist
) noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/bvh_viewer.h`

