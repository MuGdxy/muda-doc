

# Class muda::Graph



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Graph**](classmuda_1_1_graph.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Graph**](#function-graph-13) () <br> |
|   | [**Graph**](#function-graph-23) (const [**Graph**](classmuda_1_1_graph.md) &) = delete<br> |
|   | [**Graph**](#function-graph-33) ([**Graph**](classmuda_1_1_graph.md) &&) <br> |
|  void | [**add\_dependency**](#function-add_dependency) (S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; from, S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; to) <br> |
|  S&lt; [**EventRecordNode**](classmuda_1_1_event_record_node.md) &gt; | [**add\_event\_record\_node**](#function-add_event_record_node-12) (cudaEvent\_t e, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**EventRecordNode**](classmuda_1_1_event_record_node.md) &gt; | [**add\_event\_record\_node**](#function-add_event_record_node-22) (cudaEvent\_t e) <br> |
|  S&lt; [**EventWaitNode**](classmuda_1_1_event_wait_node.md) &gt; | [**add\_event\_wait\_node**](#function-add_event_wait_node-12) (cudaEvent\_t e, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**EventWaitNode**](classmuda_1_1_event_wait_node.md) &gt; | [**add\_event\_wait\_node**](#function-add_event_wait_node-22) (cudaEvent\_t e) <br> |
|  S&lt; [**HostNode**](classmuda_1_1_host_node.md) &gt; | [**add\_host\_node**](#function-add_host_node-12) (const S&lt; [**HostNodeParms**](classmuda_1_1_host_node_parms.md)&lt; T &gt; &gt; & hostParms, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**HostNode**](classmuda_1_1_host_node.md) &gt; | [**add\_host\_node**](#function-add_host_node-22) (const S&lt; [**HostNodeParms**](classmuda_1_1_host_node_parms.md)&lt; T &gt; &gt; & hostParms) <br> |
|  S&lt; [**KernelNode**](classmuda_1_1_kernel_node.md) &gt; | [**add\_kernel\_node**](#function-add_kernel_node-12) (const S&lt; [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)&lt; T &gt; &gt; & kernelParms, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**KernelNode**](classmuda_1_1_kernel_node.md) &gt; | [**add\_kernel\_node**](#function-add_kernel_node-22) (const S&lt; [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)&lt; T &gt; &gt; & kernelParms) <br> |
|  S&lt; [**MemcpyNode**](classmuda_1_1_memcpy_node.md) &gt; | [**add\_memcpy\_node**](#function-add_memcpy_node-14) (void \* dst, const void \* src, size\_t size\_bytes, cudaMemcpyKind kind, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**MemcpyNode**](classmuda_1_1_memcpy_node.md) &gt; | [**add\_memcpy\_node**](#function-add_memcpy_node-24) (void \* dst, const void \* src, size\_t size\_bytes, cudaMemcpyKind kind) <br> |
|  S&lt; [**MemcpyNode**](classmuda_1_1_memcpy_node.md) &gt; | [**add\_memcpy\_node**](#function-add_memcpy_node-34) (const cudaMemcpy3DParms & parms) <br> |
|  S&lt; [**MemcpyNode**](classmuda_1_1_memcpy_node.md) &gt; | [**add\_memcpy\_node**](#function-add_memcpy_node-44) (const cudaMemcpy3DParms & parms, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**MemsetNode**](classmuda_1_1_memset_node.md) &gt; | [**add\_memset\_node**](#function-add_memset_node-12) (const cudaMemsetParams & parms, const std::vector&lt; S&lt; [**GraphNode**](classmuda_1_1_graph_node.md) &gt; &gt; & deps) <br> |
|  S&lt; [**MemsetNode**](classmuda_1_1_memset_node.md) &gt; | [**add\_memset\_node**](#function-add_memset_node-22) (const cudaMemsetParams & parms) <br> |
|  cudaGraph\_t | [**handle**](#function-handle-12) () const<br> |
|  cudaGraph\_t | [**handle**](#function-handle-22) () <br> |
|  MUDA\_NODISCARD S&lt; [**GraphExec**](classmuda_1_1_graph_exec.md) &gt; | [**instantiate**](#function-instantiate-12) () <br> |
|  MUDA\_NODISCARD S&lt; [**GraphExec**](classmuda_1_1_graph_exec.md) &gt; | [**instantiate**](#function-instantiate-22) ([**Flags**](classmuda_1_1_flags.md)&lt; GraphInstantiateFlagBit &gt; flags) <br> |
|  [**Graph**](classmuda_1_1_graph.md) & | [**operator=**](#function-operator) (const [**Graph**](classmuda_1_1_graph.md) &) = delete<br> |
|  [**Graph**](classmuda_1_1_graph.md) & | [**operator=**](#function-operator_1) ([**Graph**](classmuda_1_1_graph.md) &&) <br> |
|   | [**~Graph**](#function-graph) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  auto | [**create**](#function-create) () <br> |


























## Public Functions Documentation




### function Graph [1/3]

```C++
muda::Graph::Graph () 
```




<hr>



### function Graph [2/3]

```C++
muda::Graph::Graph (
    const Graph &
) = delete
```




<hr>



### function Graph [3/3]

```C++
muda::Graph::Graph (
    Graph &&
) 
```




<hr>



### function add\_dependency 

```C++
void muda::Graph::add_dependency (
    S< GraphNode > from,
    S< GraphNode > to
) 
```




<hr>



### function add\_event\_record\_node [1/2]

```C++
S< EventRecordNode > muda::Graph::add_event_record_node (
    cudaEvent_t e,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_event\_record\_node [2/2]

```C++
S< EventRecordNode > muda::Graph::add_event_record_node (
    cudaEvent_t e
) 
```




<hr>



### function add\_event\_wait\_node [1/2]

```C++
S< EventWaitNode > muda::Graph::add_event_wait_node (
    cudaEvent_t e,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_event\_wait\_node [2/2]

```C++
S< EventWaitNode > muda::Graph::add_event_wait_node (
    cudaEvent_t e
) 
```




<hr>



### function add\_host\_node [1/2]

```C++
template<typename T>
S< HostNode > muda::Graph::add_host_node (
    const S< HostNodeParms < T > > & hostParms,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_host\_node [2/2]

```C++
template<typename T>
S< HostNode > muda::Graph::add_host_node (
    const S< HostNodeParms < T > > & hostParms
) 
```




<hr>



### function add\_kernel\_node [1/2]

```C++
template<typename T>
S< KernelNode > muda::Graph::add_kernel_node (
    const S< KernelNodeParms < T > > & kernelParms,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_kernel\_node [2/2]

```C++
template<typename T>
S< KernelNode > muda::Graph::add_kernel_node (
    const S< KernelNodeParms < T > > & kernelParms
) 
```




<hr>



### function add\_memcpy\_node [1/4]

```C++
S< MemcpyNode > muda::Graph::add_memcpy_node (
    void * dst,
    const void * src,
    size_t size_bytes,
    cudaMemcpyKind kind,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_memcpy\_node [2/4]

```C++
S< MemcpyNode > muda::Graph::add_memcpy_node (
    void * dst,
    const void * src,
    size_t size_bytes,
    cudaMemcpyKind kind
) 
```




<hr>



### function add\_memcpy\_node [3/4]

```C++
S< MemcpyNode > muda::Graph::add_memcpy_node (
    const cudaMemcpy3DParms & parms
) 
```




<hr>



### function add\_memcpy\_node [4/4]

```C++
S< MemcpyNode > muda::Graph::add_memcpy_node (
    const cudaMemcpy3DParms & parms,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_memset\_node [1/2]

```C++
S< MemsetNode > muda::Graph::add_memset_node (
    const cudaMemsetParams & parms,
    const std::vector< S< GraphNode > > & deps
) 
```




<hr>



### function add\_memset\_node [2/2]

```C++
S< MemsetNode > muda::Graph::add_memset_node (
    const cudaMemsetParams & parms
) 
```




<hr>



### function handle [1/2]

```C++
inline cudaGraph_t muda::Graph::handle () const
```




<hr>



### function handle [2/2]

```C++
inline cudaGraph_t muda::Graph::handle () 
```




<hr>



### function instantiate [1/2]

```C++
MUDA_NODISCARD S< GraphExec > muda::Graph::instantiate () 
```




<hr>



### function instantiate [2/2]

```C++
MUDA_NODISCARD S< GraphExec > muda::Graph::instantiate (
    Flags < GraphInstantiateFlagBit > flags
) 
```




<hr>



### function operator= 

```C++
Graph & muda::Graph::operator= (
    const Graph &
) = delete
```




<hr>



### function operator= 

```C++
Graph & muda::Graph::operator= (
    Graph &&
) 
```




<hr>



### function ~Graph 

```C++
muda::Graph::~Graph () 
```




<hr>
## Public Static Functions Documentation




### function create 

```C++
static inline auto muda::Graph::create () 
```




<hr>## Friends Documentation





### friend GraphExec 

```C++
class muda::Graph::GraphExec (
    GraphExec
) 
```




<hr>



### friend shared\_ptr&lt; Graph &gt; 

```C++
class muda::Graph::shared_ptr< Graph > (
    std::shared_ptr< Graph >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/graph.h`

