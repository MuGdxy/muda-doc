

# Class muda::details::ComputeGraphAccessor



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**ComputeGraphAccessor**](classmuda_1_1details_1_1_compute_graph_accessor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphAccessor**](#function-computegraphaccessor-13) () <br> |
|   | [**ComputeGraphAccessor**](#function-computegraphaccessor-23) ([**ComputeGraph**](classmuda_1_1_compute_graph.md) & graph) <br> |
|   | [**ComputeGraphAccessor**](#function-computegraphaccessor-33) ([**ComputeGraph**](classmuda_1_1_compute_graph.md) \* graph) <br> |
|  cudaStream\_t | [**capture\_stream**](#function-capture_stream) () const<br> |
|  void | [**check\_allow\_node\_adding**](#function-check_allow_node_adding) () const<br> |
|  void | [**check\_allow\_var\_eval**](#function-check_allow_var_eval) () const<br> |
|  auto | [**current\_closure**](#function-current_closure-12) () const<br> |
|  auto | [**current\_closure**](#function-current_closure-22) () <br> |
|  T \* | [**current\_node**](#function-current_node-13) () <br> |
|  const [**ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md) \* | [**current\_node**](#function-current_node-23) () const<br> |
|  [**ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md) \* | [**current\_node**](#function-current_node-33) () <br> |
|  cudaStream\_t | [**current\_stream**](#function-current_stream) () const<br> |
|  bool | [**is\_topo\_built**](#function-is_topo_built) () const<br> |
|  void | [**set\_capture\_node**](#function-set_capture_node) (cudaGraph\_t sub\_graph) <br> |
|  void | [**set\_event\_record\_node**](#function-set_event_record_node) (cudaEvent\_t event) <br> |
|  void | [**set\_event\_wait\_node**](#function-set_event_wait_node) (cudaEvent\_t event) <br> |
|  void | [**set\_kernel\_node**](#function-set_kernel_node) (const S&lt; [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)&lt; T &gt; &gt; & kernelParms) <br> |
|  void | [**set\_memcpy\_node**](#function-set_memcpy_node-12) (void \* dst, const void \* src, size\_t size\_bytes, cudaMemcpyKind kind) <br> |
|  void | [**set\_memcpy\_node**](#function-set_memcpy_node-22) (const cudaMemcpy3DParms & parms) <br> |
|  void | [**set\_memset\_node**](#function-set_memset_node) (const cudaMemsetParams & parms) <br> |




























## Public Functions Documentation




### function ComputeGraphAccessor [1/3]

```C++
muda::details::ComputeGraphAccessor::ComputeGraphAccessor () 
```




<hr>



### function ComputeGraphAccessor [2/3]

```C++
muda::details::ComputeGraphAccessor::ComputeGraphAccessor (
    ComputeGraph & graph
) 
```




<hr>



### function ComputeGraphAccessor [3/3]

```C++
muda::details::ComputeGraphAccessor::ComputeGraphAccessor (
    ComputeGraph * graph
) 
```




<hr>



### function capture\_stream 

```C++
cudaStream_t muda::details::ComputeGraphAccessor::capture_stream () const
```




<hr>



### function check\_allow\_node\_adding 

```C++
void muda::details::ComputeGraphAccessor::check_allow_node_adding () const
```




<hr>



### function check\_allow\_var\_eval 

```C++
void muda::details::ComputeGraphAccessor::check_allow_var_eval () const
```




<hr>



### function current\_closure [1/2]

```C++
auto muda::details::ComputeGraphAccessor::current_closure () const
```




<hr>



### function current\_closure [2/2]

```C++
auto muda::details::ComputeGraphAccessor::current_closure () 
```




<hr>



### function current\_node [1/3]

```C++
template<typename T>
T * muda::details::ComputeGraphAccessor::current_node () 
```




<hr>



### function current\_node [2/3]

```C++
const ComputeGraphNodeBase * muda::details::ComputeGraphAccessor::current_node () const
```




<hr>



### function current\_node [3/3]

```C++
ComputeGraphNodeBase * muda::details::ComputeGraphAccessor::current_node () 
```




<hr>



### function current\_stream 

```C++
cudaStream_t muda::details::ComputeGraphAccessor::current_stream () const
```




<hr>



### function is\_topo\_built 

```C++
bool muda::details::ComputeGraphAccessor::is_topo_built () const
```




<hr>



### function set\_capture\_node 

```C++
void muda::details::ComputeGraphAccessor::set_capture_node (
    cudaGraph_t sub_graph
) 
```




<hr>



### function set\_event\_record\_node 

```C++
void muda::details::ComputeGraphAccessor::set_event_record_node (
    cudaEvent_t event
) 
```




<hr>



### function set\_event\_wait\_node 

```C++
void muda::details::ComputeGraphAccessor::set_event_wait_node (
    cudaEvent_t event
) 
```




<hr>



### function set\_kernel\_node 

```C++
template<typename T>
void muda::details::ComputeGraphAccessor::set_kernel_node (
    const S< KernelNodeParms < T > > & kernelParms
) 
```




<hr>



### function set\_memcpy\_node [1/2]

```C++
void muda::details::ComputeGraphAccessor::set_memcpy_node (
    void * dst,
    const void * src,
    size_t size_bytes,
    cudaMemcpyKind kind
) 
```




<hr>



### function set\_memcpy\_node [2/2]

```C++
void muda::details::ComputeGraphAccessor::set_memcpy_node (
    const cudaMemcpy3DParms & parms
) 
```




<hr>



### function set\_memset\_node 

```C++
void muda::details::ComputeGraphAccessor::set_memset_node (
    const cudaMemsetParams & parms
) 
```




<hr>## Friends Documentation





### friend ComputeGraphVarBase 

```C++
class muda::details::ComputeGraphAccessor::ComputeGraphVarBase (
    muda::ComputeGraphVarBase
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_accessor.h`

