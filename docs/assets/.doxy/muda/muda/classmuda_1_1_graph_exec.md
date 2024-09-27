

# Class muda::GraphExec



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**GraphExec**](classmuda_1_1_graph_exec.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GraphExec**](#function-graphexec-13) () <br> |
|   | [**GraphExec**](#function-graphexec-23) (const [**GraphExec**](classmuda_1_1_graph_exec.md) &) = delete<br> |
|   | [**GraphExec**](#function-graphexec-33) ([**GraphExec**](classmuda_1_1_graph_exec.md) && other) <br> |
|  cudaGraphExec\_t | [**handle**](#function-handle) () const<br> |
|  void | [**launch**](#function-launch) (cudaStream\_t stream=nullptr) <br> |
|  [**GraphExec**](classmuda_1_1_graph_exec.md) & | [**operator=**](#function-operator) (const [**GraphExec**](classmuda_1_1_graph_exec.md) &) = delete<br> |
|  [**GraphExec**](classmuda_1_1_graph_exec.md) & | [**operator=**](#function-operator_1) ([**GraphExec**](classmuda_1_1_graph_exec.md) && other) <br> |
|  void | [**set\_event\_record\_node\_parms**](#function-set_event_record_node_parms) (S&lt; [**EventRecordNode**](classmuda_1_1_event_record_node.md) &gt; node, cudaEvent\_t event) <br> |
|  void | [**set\_event\_wait\_node\_parms**](#function-set_event_wait_node_parms) (S&lt; [**EventWaitNode**](classmuda_1_1_event_wait_node.md) &gt; node, cudaEvent\_t event) <br> |
|  void | [**set\_kernel\_node\_parms**](#function-set_kernel_node_parms) (S&lt; [**KernelNode**](classmuda_1_1_kernel_node.md) &gt; node, const S&lt; [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)&lt; T &gt; &gt; & new\_parms) <br> |
|  void | [**set\_memcpy\_node\_parms**](#function-set_memcpy_node_parms-12) (S&lt; [**MemcpyNode**](classmuda_1_1_memcpy_node.md) &gt; node, void \* dst, const void \* src, size\_t size\_bytes, cudaMemcpyKind kind) <br> |
|  void | [**set\_memcpy\_node\_parms**](#function-set_memcpy_node_parms-22) (S&lt; [**MemcpyNode**](classmuda_1_1_memcpy_node.md) &gt; node, const cudaMemcpy3DParms & parms) <br> |
|  void | [**set\_memset\_node\_parms**](#function-set_memset_node_parms) (S&lt; [**MemsetNode**](classmuda_1_1_memset_node.md) &gt; node, const cudaMemsetParams & parms) <br> |
|  void | [**upload**](#function-upload) (cudaStream\_t stream=nullptr) <br> |
|  [**GraphViewer**](classmuda_1_1_graph_viewer.md) | [**viewer**](#function-viewer) () const<br> |
|   | [**~GraphExec**](#function-graphexec) () <br> |




























## Public Functions Documentation




### function GraphExec [1/3]

```C++
muda::GraphExec::GraphExec () 
```




<hr>



### function GraphExec [2/3]

```C++
muda::GraphExec::GraphExec (
    const GraphExec &
) = delete
```




<hr>



### function GraphExec [3/3]

```C++
muda::GraphExec::GraphExec (
    GraphExec && other
) 
```




<hr>



### function handle 

```C++
inline cudaGraphExec_t muda::GraphExec::handle () const
```




<hr>



### function launch 

```C++
void muda::GraphExec::launch (
    cudaStream_t stream=nullptr
) 
```




<hr>



### function operator= 

```C++
GraphExec & muda::GraphExec::operator= (
    const GraphExec &
) = delete
```




<hr>



### function operator= 

```C++
GraphExec & muda::GraphExec::operator= (
    GraphExec && other
) 
```




<hr>



### function set\_event\_record\_node\_parms 

```C++
void muda::GraphExec::set_event_record_node_parms (
    S< EventRecordNode > node,
    cudaEvent_t event
) 
```




<hr>



### function set\_event\_wait\_node\_parms 

```C++
void muda::GraphExec::set_event_wait_node_parms (
    S< EventWaitNode > node,
    cudaEvent_t event
) 
```




<hr>



### function set\_kernel\_node\_parms 

```C++
template<typename T>
void muda::GraphExec::set_kernel_node_parms (
    S< KernelNode > node,
    const S< KernelNodeParms < T > > & new_parms
) 
```




<hr>



### function set\_memcpy\_node\_parms [1/2]

```C++
void muda::GraphExec::set_memcpy_node_parms (
    S< MemcpyNode > node,
    void * dst,
    const void * src,
    size_t size_bytes,
    cudaMemcpyKind kind
) 
```




<hr>



### function set\_memcpy\_node\_parms [2/2]

```C++
void muda::GraphExec::set_memcpy_node_parms (
    S< MemcpyNode > node,
    const cudaMemcpy3DParms & parms
) 
```




<hr>



### function set\_memset\_node\_parms 

```C++
void muda::GraphExec::set_memset_node_parms (
    S< MemsetNode > node,
    const cudaMemsetParams & parms
) 
```




<hr>



### function upload 

```C++
void muda::GraphExec::upload (
    cudaStream_t stream=nullptr
) 
```




<hr>



### function viewer 

```C++
GraphViewer muda::GraphExec::viewer () const
```




<hr>



### function ~GraphExec 

```C++
muda::GraphExec::~GraphExec () 
```




<hr>## Friends Documentation





### friend Graph 

```C++
class muda::GraphExec::Graph (
    Graph
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/graph_exec.h`

