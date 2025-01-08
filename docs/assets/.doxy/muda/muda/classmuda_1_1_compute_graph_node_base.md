

# Class muda::ComputeGraphNodeBase



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md)










Inherited by the following classes: [muda::ComputeGraphNode](classmuda_1_1_compute_graph_node.md),  [muda::ComputeGraphNode](classmuda_1_1_compute_graph_node.md),  [muda::ComputeGraphNode](classmuda_1_1_compute_graph_node.md),  [muda::ComputeGraphNode](classmuda_1_1_compute_graph_node.md),  [muda::ComputeGraphNode](classmuda_1_1_compute_graph_node.md),  [muda::ComputeGraphCaptureNode](classmuda_1_1_compute_graph_capture_node.md),  [muda::ComputeGraphNode](classmuda_1_1_compute_graph_node.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  auto | [**access\_index**](#function-access_index) () const<br> |
|  auto | [**name**](#function-name) () const<br> |
|  auto | [**node\_id**](#function-node_id) () const<br> |
|  auto | [**type**](#function-type) () const<br> |
| virtual  | [**~ComputeGraphNodeBase**](#function-computegraphnodebase) () = default<br> |




## Protected Types

| Type | Name |
| ---: | :--- |
| typedef std::shared\_ptr&lt; T &gt; | [**S**](#typedef-s)  <br> |




## Protected Attributes

| Type | Name |
| ---: | :--- |
|  uint64\_t | [**m\_access\_index**](#variable-m_access_index)  <br> |
|  cudaGraphNode\_t | [**m\_cuda\_node**](#variable-m_cuda_node)   = = nullptr<br> |
|  std::string | [**m\_name**](#variable-m_name)  <br> |
|  [**NodeId**](classmuda_1_1_node_id.md) | [**m\_node\_id**](#variable-m_node_id)  <br> |
|  ComputeGraphNodeType | [**m\_type**](#variable-m_type)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphNodeBase**](#function-computegraphnodebase) (std::string\_view name, [**NodeId**](classmuda_1_1_node_id.md) node\_id, uint64\_t access\_index, ComputeGraphNodeType type) <br> |
|  auto | [**handle**](#function-handle) () const<br> |
|  auto | [**is\_valid**](#function-is_valid) () const<br> |
|  void | [**set\_handle**](#function-set_handle) (cudaGraphNode\_t handle) <br> |




## Public Functions Documentation




### function access\_index 

```C++
inline auto muda::ComputeGraphNodeBase::access_index () const
```




<hr>



### function name 

```C++
inline auto muda::ComputeGraphNodeBase::name () const
```




<hr>



### function node\_id 

```C++
inline auto muda::ComputeGraphNodeBase::node_id () const
```




<hr>



### function type 

```C++
inline auto muda::ComputeGraphNodeBase::type () const
```




<hr>



### function ~ComputeGraphNodeBase 

```C++
virtual muda::ComputeGraphNodeBase::~ComputeGraphNodeBase () = default
```




<hr>
## Protected Types Documentation




### typedef S 

```C++
using muda::ComputeGraphNodeBase::S =  std::shared_ptr<T>;
```




<hr>
## Protected Attributes Documentation




### variable m\_access\_index 

```C++
uint64_t muda::ComputeGraphNodeBase::m_access_index;
```




<hr>



### variable m\_cuda\_node 

```C++
cudaGraphNode_t muda::ComputeGraphNodeBase::m_cuda_node;
```




<hr>



### variable m\_name 

```C++
std::string muda::ComputeGraphNodeBase::m_name;
```




<hr>



### variable m\_node\_id 

```C++
NodeId muda::ComputeGraphNodeBase::m_node_id;
```




<hr>



### variable m\_type 

```C++
ComputeGraphNodeType muda::ComputeGraphNodeBase::m_type;
```




<hr>
## Protected Functions Documentation




### function ComputeGraphNodeBase 

```C++
inline muda::ComputeGraphNodeBase::ComputeGraphNodeBase (
    std::string_view name,
    NodeId node_id,
    uint64_t access_index,
    ComputeGraphNodeType type
) 
```




<hr>



### function handle 

```C++
inline auto muda::ComputeGraphNodeBase::handle () const
```




<hr>



### function is\_valid 

```C++
inline auto muda::ComputeGraphNodeBase::is_valid () const
```




<hr>



### function set\_handle 

```C++
inline void muda::ComputeGraphNodeBase::set_handle (
    cudaGraphNode_t handle
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_node.h`

