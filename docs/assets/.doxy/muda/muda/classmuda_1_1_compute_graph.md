

# Class muda::ComputeGraph



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraph**](classmuda_1_1_compute_graph.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**AddNodeProxy**](classmuda_1_1_compute_graph_1_1_add_node_proxy.md) <br> |
| class | [**GraphPhaseGuard**](classmuda_1_1_compute_graph_1_1_graph_phase_guard.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**ComputeGraphDependency**](classmuda_1_1_compute_graph_dependency.md) | [**Dependency**](#typedef-dependency)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraph**](#function-computegraph-13) (const [**ComputeGraph**](classmuda_1_1_compute_graph.md) &) = delete<br> |
|   | [**ComputeGraph**](#function-computegraph-23) ([**ComputeGraph**](classmuda_1_1_compute_graph.md) &&) = delete<br> |
|   | [**ComputeGraph**](#function-computegraph-33) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) & manager, std::string\_view name="graph", ComputeGraphFlag flag=ComputeGraphFlag::HostLaunch) <br> |
|  void | [**build**](#function-build) () <br> |
|  void | [**capture**](#function-capture-12) (std::function&lt; void(cudaStream\_t)&gt; && f) <br> |
|  void | [**capture**](#function-capture-22) (std::string\_view name, std::function&lt; void(cudaStream\_t)&gt; && f) <br> |
|  [**AddNodeProxy**](classmuda_1_1_compute_graph_1_1_add_node_proxy.md) | [**create\_node**](#function-create_node) (std::string\_view node\_name) <br> |
|  void | [**graphviz**](#function-graphviz) (std::ostream & o, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options={}) <br> |
|  void | [**launch**](#function-launch-12) (bool single\_stream, cudaStream\_t s=nullptr) <br> |
|  void | [**launch**](#function-launch-22) (cudaStream\_t s=nullptr) <br> |
|  std::string\_view | [**name**](#function-name) () const<br> |
|   | [**operator GraphViewer**](#function-operator-graphviewer) () <br> |
|  [**ComputeGraph**](classmuda_1_1_compute_graph.md) & | [**operator=**](#function-operator) (const [**ComputeGraph**](classmuda_1_1_compute_graph.md) &) = delete<br> |
|  [**ComputeGraph**](classmuda_1_1_compute_graph.md) & | [**operator=**](#function-operator_1) ([**ComputeGraph**](classmuda_1_1_compute_graph.md) &&) = delete<br> |
|  [**Event::QueryResult**](classmuda_1_1_event.md#enum-queryresult) | [**query**](#function-query) () const<br> |
|  void | [**update**](#function-update) () <br> |
|  [**GraphViewer**](classmuda_1_1_graph_viewer.md) | [**viewer**](#function-viewer) () <br> |
|   | [**~ComputeGraph**](#function-computegraph) () <br> |




























## Public Types Documentation




### typedef Dependency 

```C++
using muda::ComputeGraph::Dependency =  ComputeGraphDependency;
```




<hr>
## Public Functions Documentation




### function ComputeGraph [1/3]

```C++
muda::ComputeGraph::ComputeGraph (
    const ComputeGraph &
) = delete
```




<hr>



### function ComputeGraph [2/3]

```C++
muda::ComputeGraph::ComputeGraph (
    ComputeGraph &&
) = delete
```




<hr>



### function ComputeGraph [3/3]

```C++
muda::ComputeGraph::ComputeGraph (
    ComputeGraphVarManager & manager,
    std::string_view name="graph",
    ComputeGraphFlag flag=ComputeGraphFlag::HostLaunch
) 
```




<hr>



### function build 

```C++
void muda::ComputeGraph::build () 
```




<hr>



### function capture [1/2]

```C++
void muda::ComputeGraph::capture (
    std::function< void(cudaStream_t)> && f
) 
```




<hr>



### function capture [2/2]

```C++
void muda::ComputeGraph::capture (
    std::string_view name,
    std::function< void(cudaStream_t)> && f
) 
```




<hr>



### function create\_node 

```C++
AddNodeProxy muda::ComputeGraph::create_node (
    std::string_view node_name
) 
```




<hr>



### function graphviz 

```C++
void muda::ComputeGraph::graphviz (
    std::ostream & o,
    const ComputeGraphGraphvizOptions & options={}
) 
```




<hr>



### function launch [1/2]

```C++
void muda::ComputeGraph::launch (
    bool single_stream,
    cudaStream_t s=nullptr
) 
```




<hr>



### function launch [2/2]

```C++
inline void muda::ComputeGraph::launch (
    cudaStream_t s=nullptr
) 
```




<hr>



### function name 

```C++
inline std::string_view muda::ComputeGraph::name () const
```




<hr>



### function operator GraphViewer 

```C++
inline muda::ComputeGraph::operator GraphViewer () 
```




<hr>



### function operator= 

```C++
ComputeGraph & muda::ComputeGraph::operator= (
    const ComputeGraph &
) = delete
```




<hr>



### function operator= 

```C++
ComputeGraph & muda::ComputeGraph::operator= (
    ComputeGraph &&
) = delete
```




<hr>



### function query 

```C++
Event::QueryResult muda::ComputeGraph::query () const
```




<hr>



### function update 

```C++
void muda::ComputeGraph::update () 
```




<hr>



### function viewer 

```C++
GraphViewer muda::ComputeGraph::viewer () 
```




<hr>



### function ~ComputeGraph 

```C++
muda::ComputeGraph::~ComputeGraph () 
```




<hr>## Friends Documentation





### friend ComputeGraphAccessor 

```C++
class muda::ComputeGraph::ComputeGraphAccessor (
    muda::details::ComputeGraphAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph.h`

