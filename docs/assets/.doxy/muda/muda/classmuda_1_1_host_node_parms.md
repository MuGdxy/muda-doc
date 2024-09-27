

# Class muda::HostNodeParms

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**HostNodeParms**](classmuda_1_1_host_node_parms.md)








Inherits the following classes: [muda::NodeParms](classmuda_1_1_node_parms.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**HostNodeParms**](classmuda_1_1_host_node_parms.md) | [**this\_type**](#typedef-this_type)  <br> |








## Public Attributes

| Type | Name |
| ---: | :--- |
|  T | [**hostData**](#variable-hostdata)  <br> |
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**HostNodeParms**](#function-hostnodeparms) (const T & f) <br> |
|  auto | [**fn**](#function-fn-12) () const<br> |
|  void | [**fn**](#function-fn-22) (cudaHostFn\_t fn) <br> |
|  const cudaHostNodeParams \* | [**handle**](#function-handle-12) () const<br> |
|  cudaHostNodeParams \* | [**handle**](#function-handle-22) () <br> |
|  auto | [**userdata**](#function-userdata-12) () const<br> |
|  void | [**userdata**](#function-userdata-22) (void \* userdata) <br> |


## Public Functions inherited from muda::NodeParms

See [muda::NodeParms](classmuda_1_1_node_parms.md)

| Type | Name |
| ---: | :--- |
|   | [**NodeParms**](classmuda_1_1_node_parms.md#function-nodeparms) () = default<br> |
| virtual  | [**~NodeParms**](classmuda_1_1_node_parms.md#function-nodeparms) () = default<br> |






















































## Public Types Documentation




### typedef this\_type 

```C++
using muda::HostNodeParms< T >::this_type =  HostNodeParms;
```




<hr>
## Public Attributes Documentation




### variable hostData 

```C++
T muda::HostNodeParms< T >::hostData;
```




<hr>
## Public Functions Documentation




### function HostNodeParms 

```C++
inline muda::HostNodeParms::HostNodeParms (
    const T & f
) 
```




<hr>



### function fn [1/2]

```C++
inline auto muda::HostNodeParms::fn () const
```




<hr>



### function fn [2/2]

```C++
inline void muda::HostNodeParms::fn (
    cudaHostFn_t fn
) 
```




<hr>



### function handle [1/2]

```C++
inline const cudaHostNodeParams * muda::HostNodeParms::handle () const
```




<hr>



### function handle [2/2]

```C++
inline cudaHostNodeParams * muda::HostNodeParms::handle () 
```




<hr>



### function userdata [1/2]

```C++
inline auto muda::HostNodeParms::userdata () const
```




<hr>



### function userdata [2/2]

```C++
inline void muda::HostNodeParms::userdata (
    void * userdata
) 
```




<hr>## Friends Documentation





### friend Graph 

```C++
class muda::HostNodeParms::Graph (
    Graph
) 
```




<hr>



### friend shared\_ptr&lt; this\_type &gt; 

```C++
class muda::HostNodeParms::shared_ptr< this_type > (
    std::shared_ptr< this_type >
) 
```




<hr>



### friend unique\_ptr&lt; this\_type &gt; 

```C++
class muda::HostNodeParms::unique_ptr< this_type > (
    std::unique_ptr< this_type >
) 
```




<hr>



### friend weak\_ptr&lt; this\_type &gt; 

```C++
class muda::HostNodeParms::weak_ptr< this_type > (
    std::weak_ptr< this_type >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/host_node.h`

