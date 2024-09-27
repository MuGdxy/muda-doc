

# Class muda::GraphNode



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**GraphNode**](classmuda_1_1_graph_node.md)










Inherited by the following classes: [muda::EventRecordNode](classmuda_1_1_event_record_node.md),  [muda::EventWaitNode](classmuda_1_1_event_wait_node.md),  [muda::HostNode](classmuda_1_1_host_node.md),  [muda::KernelNode](classmuda_1_1_kernel_node.md),  [muda::MemcpyNode](classmuda_1_1_memcpy_node.md),  [muda::MemsetNode](classmuda_1_1_memset_node.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**GraphNode**](classmuda_1_1_graph_node.md) | [**this\_type**](#typedef-this_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GraphNode**](#function-graphnode) () <br> |
|  cudaGraphNode\_t | [**handle**](#function-handle) () const<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  cudaGraphNode\_t | [**m\_handle**](#variable-m_handle)  <br> |




















## Public Types Documentation




### typedef this\_type 

```C++
using muda::GraphNode::this_type =  GraphNode;
```




<hr>
## Public Functions Documentation




### function GraphNode 

```C++
inline muda::GraphNode::GraphNode () 
```




<hr>



### function handle 

```C++
inline cudaGraphNode_t muda::GraphNode::handle () const
```




<hr>
## Protected Attributes Documentation




### variable m\_handle 

```C++
cudaGraphNode_t muda::GraphNode::m_handle;
```




<hr>## Friends Documentation





### friend Graph 

```C++
class muda::GraphNode::Graph (
    Graph
) 
```




<hr>



### friend GraphExec 

```C++
class muda::GraphNode::GraphExec (
    GraphExec
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/graph_base.h`

