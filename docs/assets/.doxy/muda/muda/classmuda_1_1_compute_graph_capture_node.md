

# Class muda::ComputeGraphCaptureNode



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphCaptureNode**](classmuda_1_1_compute_graph_capture_node.md)








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
|  cudaGraph\_t | [**m\_sub\_graph**](#variable-m_sub_graph)   = = nullptr<br> |


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
|   | [**ComputeGraphCaptureNode**](#function-computegraphcapturenode) ([**NodeId**](classmuda_1_1_node_id.md) node\_id, uint64\_t access\_index) <br> |
|  void | [**set\_node**](#function-set_node) (cudaGraphNode\_t node) <br> |
|  void | [**update\_sub\_graph**](#function-update_sub_graph) (cudaGraph\_t sub\_graph) <br> |
| virtual  | [**~ComputeGraphCaptureNode**](#function-computegraphcapturenode) () override<br> |


## Protected Functions inherited from muda::ComputeGraphNodeBase

See [muda::ComputeGraphNodeBase](classmuda_1_1_compute_graph_node_base.md)

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md#function-computegraphnodebase) (std::string\_view name, [**NodeId**](classmuda_1_1_node_id.md) node\_id, uint64\_t access\_index, ComputeGraphNodeType type) <br> |
|  auto | [**handle**](classmuda_1_1_compute_graph_node_base.md#function-handle) () const<br> |
|  auto | [**is\_valid**](classmuda_1_1_compute_graph_node_base.md#function-is_valid) () const<br> |
|  void | [**set\_handle**](classmuda_1_1_compute_graph_node_base.md#function-set_handle) (cudaGraphNode\_t handle) <br> |






## Protected Attributes Documentation




### variable m\_sub\_graph 

```C++
cudaGraph_t muda::ComputeGraphCaptureNode::m_sub_graph;
```




<hr>
## Protected Functions Documentation




### function ComputeGraphCaptureNode 

```C++
inline muda::ComputeGraphCaptureNode::ComputeGraphCaptureNode (
    NodeId node_id,
    uint64_t access_index
) 
```




<hr>



### function set\_node 

```C++
inline void muda::ComputeGraphCaptureNode::set_node (
    cudaGraphNode_t node
) 
```




<hr>



### function update\_sub\_graph 

```C++
inline void muda::ComputeGraphCaptureNode::update_sub_graph (
    cudaGraph_t sub_graph
) 
```




<hr>



### function ~ComputeGraphCaptureNode 

```C++
inline virtual muda::ComputeGraphCaptureNode::~ComputeGraphCaptureNode () override
```




<hr>## Friends Documentation





### friend ComputeGraphAccessor 

```C++
class muda::ComputeGraphCaptureNode::ComputeGraphAccessor (
    details::ComputeGraphAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/nodes/compute_graph_catpure_node.h`

