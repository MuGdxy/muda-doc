

# Class muda::KernelNodeParms

**template &lt;typename U&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)








Inherits the following classes: [muda::NodeParms](classmuda_1_1_node_parms.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md) | [**this\_type**](#typedef-this_type)  <br> |








## Public Attributes

| Type | Name |
| ---: | :--- |
|  U | [**kernelParmData**](#variable-kernelparmdata)  <br> |
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**KernelNodeParms**](#function-kernelnodeparms-12) (Args &&... args) <br> |
|   | [**KernelNodeParms**](#function-kernelnodeparms-22) () <br> |
|  auto | [**block\_dim**](#function-block_dim-12) () <br> |
|  void | [**block\_dim**](#function-block_dim-22) (const dim3 & v) <br> |
|  auto | [**extra**](#function-extra-12) () <br> |
|  void | [**extra**](#function-extra-22) (void \*\* v) <br> |
|  auto | [**func**](#function-func-12) () <br> |
|  void | [**func**](#function-func-22) (void \* v) <br> |
|  auto | [**grid\_dim**](#function-grid_dim-12) () <br> |
|  void | [**grid\_dim**](#function-grid_dim-22) (const dim3 & v) <br> |
|  const cudaKernelNodeParams \* | [**handle**](#function-handle) () const<br> |
|  auto | [**kernel\_params**](#function-kernel_params-12) () <br> |
|  void | [**kernel\_params**](#function-kernel_params-22) (const std::vector&lt; void \* &gt; & v) <br> |
|  void | [**parse**](#function-parse) (std::function&lt; std::vector&lt; void \* &gt;(U &)&gt; pred) <br> |
|  auto | [**shared\_mem\_bytes**](#function-shared_mem_bytes-12) () <br> |
|  void | [**shared\_mem\_bytes**](#function-shared_mem_bytes-22) (unsigned int v) <br> |


## Public Functions inherited from muda::NodeParms

See [muda::NodeParms](classmuda_1_1_node_parms.md)

| Type | Name |
| ---: | :--- |
|   | [**NodeParms**](classmuda_1_1_node_parms.md#function-nodeparms) () = default<br> |
| virtual  | [**~NodeParms**](classmuda_1_1_node_parms.md#function-nodeparms) () = default<br> |






















































## Public Types Documentation




### typedef this\_type 

```C++
using muda::KernelNodeParms< U >::this_type =  KernelNodeParms;
```




<hr>
## Public Attributes Documentation




### variable kernelParmData 

```C++
U muda::KernelNodeParms< U >::kernelParmData;
```




<hr>
## Public Functions Documentation




### function KernelNodeParms [1/2]

```C++
template<typename... Args>
inline muda::KernelNodeParms::KernelNodeParms (
    Args &&... args
) 
```




<hr>



### function KernelNodeParms [2/2]

```C++
inline muda::KernelNodeParms::KernelNodeParms () 
```




<hr>



### function block\_dim [1/2]

```C++
inline auto muda::KernelNodeParms::block_dim () 
```




<hr>



### function block\_dim [2/2]

```C++
inline void muda::KernelNodeParms::block_dim (
    const dim3 & v
) 
```




<hr>



### function extra [1/2]

```C++
inline auto muda::KernelNodeParms::extra () 
```




<hr>



### function extra [2/2]

```C++
inline void muda::KernelNodeParms::extra (
    void ** v
) 
```




<hr>



### function func [1/2]

```C++
inline auto muda::KernelNodeParms::func () 
```




<hr>



### function func [2/2]

```C++
inline void muda::KernelNodeParms::func (
    void * v
) 
```




<hr>



### function grid\_dim [1/2]

```C++
inline auto muda::KernelNodeParms::grid_dim () 
```




<hr>



### function grid\_dim [2/2]

```C++
inline void muda::KernelNodeParms::grid_dim (
    const dim3 & v
) 
```




<hr>



### function handle 

```C++
inline const cudaKernelNodeParams * muda::KernelNodeParms::handle () const
```




<hr>



### function kernel\_params [1/2]

```C++
inline auto muda::KernelNodeParms::kernel_params () 
```




<hr>



### function kernel\_params [2/2]

```C++
inline void muda::KernelNodeParms::kernel_params (
    const std::vector< void * > & v
) 
```




<hr>



### function parse 

```C++
inline void muda::KernelNodeParms::parse (
    std::function< std::vector< void * >(U &)> pred
) 
```




<hr>



### function shared\_mem\_bytes [1/2]

```C++
inline auto muda::KernelNodeParms::shared_mem_bytes () 
```




<hr>



### function shared\_mem\_bytes [2/2]

```C++
inline void muda::KernelNodeParms::shared_mem_bytes (
    unsigned int v
) 
```




<hr>## Friends Documentation





### friend Graph 

```C++
class muda::KernelNodeParms::Graph (
    Graph
) 
```




<hr>



### friend shared\_ptr&lt; this\_type &gt; 

```C++
class muda::KernelNodeParms::shared_ptr< this_type > (
    std::shared_ptr< this_type >
) 
```




<hr>



### friend unique\_ptr&lt; this\_type &gt; 

```C++
class muda::KernelNodeParms::unique_ptr< this_type > (
    std::unique_ptr< this_type >
) 
```




<hr>



### friend weak\_ptr&lt; this\_type &gt; 

```C++
class muda::KernelNodeParms::weak_ptr< this_type > (
    std::weak_ptr< this_type >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/kernel_node.h`

