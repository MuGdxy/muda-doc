

# Class muda::ComputeGraphNode

**template &lt;typename NodeT, ComputeGraphNodeType Type&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphNode**](classmuda_1_1_compute_graph_node.md)








Inherits the following classes: [muda::ComputeGraphNodeBase](classmuda_1_1_compute_graph_node_base.md)
























































## Public Functions inherited from muda::ComputeGraphNodeBase

See [muda::ComputeGraphNodeBase](classmuda_1_1_compute_graph_node_base.md)

| Type | Name |
| ---: | :--- |
|  auto | [**access\_index**](classmuda_1_1_compute_graph_node_base.md#function-access_index) () const<br> |
|  auto | [**name**](classmuda_1_1_compute_graph_node_base.md#function-name) () const<br> |
|  auto | [**node\_id**](classmuda_1_1_compute_graph_node_base.md#function-node_id) () const<br> |
|  auto | [**type**](classmuda_1_1_compute_graph_node_base.md#function-type) () const<br> |
| virtual  | [**~ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md#function-computegraphnodebase) () = default<br> |








## Protected Types inherited from muda::ComputeGraphNodeBase

See [muda::ComputeGraphNodeBase](classmuda_1_1_compute_graph_node_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::shared\_ptr&lt; T &gt; | [**S**](classmuda_1_1_compute_graph_node_base.md#typedef-s)  <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  S&lt; NodeT &gt; | [**m\_node**](#variable-m_node)  <br> |


## Protected Attributes inherited from muda::ComputeGraphNodeBase

See [muda::ComputeGraphNodeBase](classmuda_1_1_compute_graph_node_base.md)

| Type | Name |
| ---: | :--- |
|  uint64\_t | [**m\_access\_index**](classmuda_1_1_compute_graph_node_base.md#variable-m_access_index)  <br> |
|  cudaGraphNode\_t | [**m\_cuda\_node**](classmuda_1_1_compute_graph_node_base.md#variable-m_cuda_node)   = = nullptr<br> |
|  std::string | [**m\_name**](classmuda_1_1_compute_graph_node_base.md#variable-m_name)  <br> |
|  [**NodeId**](classmuda_1_1_node_id.md) | [**m\_node\_id**](classmuda_1_1_compute_graph_node_base.md#variable-m_node_id)  <br> |
|  ComputeGraphNodeType | [**m\_type**](classmuda_1_1_compute_graph_node_base.md#variable-m_type)  <br> |






























## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphNode**](#function-computegraphnode) ([**NodeId**](classmuda_1_1_node_id.md) node\_id, uint64\_t access\_graph\_index) <br> |
|  void | [**set\_node**](#function-set_node) (S&lt; NodeT &gt; node) <br> |
| virtual  | [**~ComputeGraphNode**](#function-computegraphnode) () = default<br> |


## Protected Functions inherited from muda::ComputeGraphNodeBase

See [muda::ComputeGraphNodeBase](classmuda_1_1_compute_graph_node_base.md)

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md#function-computegraphnodebase) (std::string\_view name, [**NodeId**](classmuda_1_1_node_id.md) node\_id, uint64\_t access\_index, ComputeGraphNodeType type) <br> |
|  auto | [**handle**](classmuda_1_1_compute_graph_node_base.md#function-handle) () const<br> |
|  auto | [**is\_valid**](classmuda_1_1_compute_graph_node_base.md#function-is_valid) () const<br> |
|  void | [**set\_handle**](classmuda_1_1_compute_graph_node_base.md#function-set_handle) (cudaGraphNode\_t handle) <br> |






## Protected Attributes Documentation




### variable m\_node 

```C++
S<NodeT> muda::ComputeGraphNode< NodeT, Type >::m_node;
```




<hr>
## Protected Functions Documentation




### function ComputeGraphNode 

```C++
muda::ComputeGraphNode::ComputeGraphNode (
    NodeId node_id,
    uint64_t access_graph_index
) 
```




<hr>



### function set\_node 

```C++
void muda::ComputeGraphNode::set_node (
    S< NodeT > node
) 
```




<hr>



### function ~ComputeGraphNode 

```C++
virtual muda::ComputeGraphNode::~ComputeGraphNode () = default
```




<hr>## Friends Documentation





### friend ComputeGraphAccessor 

```C++
class muda::ComputeGraphNode::ComputeGraphAccessor (
    details::ComputeGraphAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_node.h`

