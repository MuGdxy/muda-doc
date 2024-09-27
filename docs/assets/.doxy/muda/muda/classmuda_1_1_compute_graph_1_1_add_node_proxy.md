

# Class muda::ComputeGraph::AddNodeProxy



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraph**](classmuda_1_1_compute_graph.md) **>** [**AddNodeProxy**](classmuda_1_1_compute_graph_1_1_add_node_proxy.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AddNodeProxy**](#function-addnodeproxy) ([**ComputeGraph**](classmuda_1_1_compute_graph.md) & cg, std::string\_view node\_name) <br> |
|  [**ComputeGraph**](classmuda_1_1_compute_graph.md) & | [**operator&lt;&lt;**](#function-operator) (std::function&lt; void()&gt; && f) <br> |




























## Public Functions Documentation




### function AddNodeProxy 

```C++
muda::ComputeGraph::AddNodeProxy::AddNodeProxy (
    ComputeGraph & cg,
    std::string_view node_name
) 
```




<hr>



### function operator&lt;&lt; 

```C++
ComputeGraph & muda::ComputeGraph::AddNodeProxy::operator<< (
    std::function< void()> && f
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph.h`

