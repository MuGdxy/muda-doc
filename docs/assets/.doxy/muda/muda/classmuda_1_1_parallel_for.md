

# Class muda::ParallelFor



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ParallelFor**](classmuda_1_1_parallel_for.md)



_a frequently used parallel for loop,_ **DynamicBlockDim** _and_**GridStrideLoop** _strategy are provided, and can be switched seamlessly to each other._

* `#include <parallel_for.h>`



Inherits the following classes: [muda::LaunchBase](classmuda_1_1_launch_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)&lt; [**details::ParallelForCallable**](classmuda_1_1details_1_1_parallel_for_callable.md)&lt; raw\_type\_t&lt; F &gt; &gt; &gt; | [**NodeParms**](#typedef-nodeparms)  <br> |


## Public Types inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](classmuda_1_1_launch_base.md#typedef-derived_type)  <br> |


























































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST | [**ParallelFor**](#function-parallelfor-13) (size\_t shared\_mem\_size=0, cudaStream\_t stream=nullptr) <br>_Calculate grid dim automatically to cover the range, automatially choose the block size to achieve max occupancy._  |
|  MUDA\_HOST | [**ParallelFor**](#function-parallelfor-23) (int blockDim, size\_t shared\_mem\_size=0, cudaStream\_t stream=nullptr) <br>_Calculate grid dim automatically to cover the range, but you need mannally set the block size._  |
|  MUDA\_HOST | [**ParallelFor**](#function-parallelfor-33) (int gridDim, int blockDim, size\_t shared\_mem\_size=0, cudaStream\_t stream=nullptr) <br>_Use Gride Stride Loop to cover the range, you need mannally set the grid size and block size. Gride Stride Loop: if grid\_dim \* block\_dim &lt; count, there will be a loop in every thread, to process multiple indices._  |
|  MUDA\_HOST [**ParallelFor**](classmuda_1_1_parallel_for.md) & | [**apply**](#function-apply-12) (int count, F && f) <br> |
|  MUDA\_HOST [**ParallelFor**](classmuda_1_1_parallel_for.md) & | [**apply**](#function-apply-22) (int count, F && f, [**Tag**](structmuda_1_1_tag.md)&lt; UserTag &gt;) <br> |
|  MUDA\_HOST MUDA\_NODISCARD auto | [**as\_node\_parms**](#function-as_node_parms-12) (int count, F && f) <br> |
|  MUDA\_HOST MUDA\_NODISCARD auto | [**as\_node\_parms**](#function-as_node_parms-22) (int count, F && f, [**Tag**](structmuda_1_1_tag.md)&lt; UserTag &gt;) <br> |
|  MUDA\_GENERIC int | [**calculate\_block\_dim**](#function-calculate_block_dim) (int count) const<br> |
|  MUDA\_GENERIC int | [**calculate\_grid\_dim**](#function-calculate_grid_dim-12) (int count) const<br> |
|  MUDA\_GENERIC void | [**check\_input**](#function-check_input) (int count) const<br> |
|  MUDA\_HOST void | [**invoke**](#function-invoke) (int count, F && f) <br> |


## Public Functions inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**LaunchBase**](classmuda_1_1_launch_base.md#function-launchbase-22) (::cudaStream\_t stream) <br> |
|  T & | [**callback**](classmuda_1_1_launch_base.md#function-callback) (const std::function&lt; void(::cudaStream\_t, ::cudaError)&gt; & callback) <br> |
|  T & | [**file\_line**](classmuda_1_1_launch_base.md#function-file_line) (std::string\_view file, int line) <br> |
|  T & | [**kernel\_name**](classmuda_1_1_launch_base.md#function-kernel_name) (std::string\_view name) <br> |
|  Next | [**next**](classmuda_1_1_launch_base.md#function-next-12) (Next n) <br> |
|  Next | [**next**](classmuda_1_1_launch_base.md#function-next-22) (Args &&... args) <br> |
|  T & | [**pop\_range**](classmuda_1_1_launch_base.md#function-pop_range) () <br> |
|  T & | [**push\_range**](classmuda_1_1_launch_base.md#function-push_range) (const std::string & name) <br> |
|  T & | [**record**](classmuda_1_1_launch_base.md#function-record-13) (cudaEvent\_t e, int flag=cudaEventRecordDefault) <br> |
|  T & | [**record**](classmuda_1_1_launch_base.md#function-record-23) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  T & | [**record**](classmuda_1_1_launch_base.md#function-record-33) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  T & | [**wait**](classmuda_1_1_launch_base.md#function-wait-14) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|  T & | [**wait**](classmuda_1_1_launch_base.md#function-wait-24) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  T & | [**wait**](classmuda_1_1_launch_base.md#function-wait-34) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  T & | [**wait**](classmuda_1_1_launch_base.md#function-wait-44) () <br> |
|  T & | [**when**](classmuda_1_1_launch_base.md#function-when) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|   | [**~LaunchBase**](classmuda_1_1_launch_base.md#function-launchbase) () <br> |


## Public Functions inherited from muda::LaunchCore

See [muda::LaunchCore](classmuda_1_1_launch_core.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**LaunchCore**](classmuda_1_1_launch_core.md#function-launchcore) (::cudaStream\_t stream) <br> |
|  void | [**callback**](classmuda_1_1_launch_core.md#function-callback) (const std::function&lt; void(::cudaStream\_t, ::cudaError)&gt; & callback) <br> |
|  void | [**init\_stream**](classmuda_1_1_launch_core.md#function-init_stream) (::cudaStream\_t s) <br> |
|  void | [**pop\_range**](classmuda_1_1_launch_core.md#function-pop_range) () <br> |
|  void | [**push\_range**](classmuda_1_1_launch_core.md#function-push_range) (const std::string & name) <br> |
|  void | [**record**](classmuda_1_1_launch_core.md#function-record-13) (cudaEvent\_t e, int flag=cudaEventRecordDefault) <br> |
|  void | [**record**](classmuda_1_1_launch_core.md#function-record-23) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  void | [**record**](classmuda_1_1_launch_core.md#function-record-33) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  void | [**wait**](classmuda_1_1_launch_core.md#function-wait-14) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|  void | [**wait**](classmuda_1_1_launch_core.md#function-wait-24) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  void | [**wait**](classmuda_1_1_launch_core.md#function-wait-34) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  void | [**wait**](classmuda_1_1_launch_core.md#function-wait-44) () <br> |
|  void | [**when**](classmuda_1_1_launch_core.md#function-when) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|   | [**~LaunchCore**](classmuda_1_1_launch_core.md#function-launchcore) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC int | [**calculate\_grid\_dim**](#function-calculate_grid_dim-22) (int count, int block\_dim) <br> |
|  MUDA\_GENERIC static MUDA\_NODISCARD int | [**round\_up\_blocks**](#function-round_up_blocks) (int count, int block\_dim) <br> |




## Public Static Functions inherited from muda::LaunchCore

See [muda::LaunchCore](classmuda_1_1_launch_core.md)

| Type | Name |
| ---: | :--- |
|  void | [**file\_line**](classmuda_1_1_launch_core.md#function-file_line) (std::string\_view file, int line) <br> |
|  void | [**kernel\_name**](classmuda_1_1_launch_core.md#function-kernel_name) (std::string\_view name) <br> |
|  void | [**wait\_device**](classmuda_1_1_launch_core.md#function-wait_device) () <br> |
|  void | [**wait\_event**](classmuda_1_1_launch_core.md#function-wait_event) (cudaEvent\_t event) <br> |
|  void | [**wait\_stream**](classmuda_1_1_launch_core.md#function-wait_stream) (::cudaStream\_t stream) <br> |






## Protected Types inherited from muda::LaunchCore

See [muda::LaunchCore](classmuda_1_1_launch_core.md)

| Type | Name |
| ---: | :--- |
| typedef std::shared\_ptr&lt; T &gt; | [**S**](classmuda_1_1_launch_core.md#typedef-s)  <br> |












## Protected Attributes inherited from muda::LaunchCore

See [muda::LaunchCore](classmuda_1_1_launch_core.md)

| Type | Name |
| ---: | :--- |
|  ::cudaStream\_t | [**m\_stream**](classmuda_1_1_launch_core.md#variable-m_stream)  <br> |














































## Protected Functions inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
|  T & | [**pop\_kernel\_label**](classmuda_1_1_launch_base.md#function-pop_kernel_label) () <br> |


## Protected Functions inherited from muda::LaunchCore

See [muda::LaunchCore](classmuda_1_1_launch_core.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST void | [**pop\_kernel\_label**](classmuda_1_1_launch_core.md#function-pop_kernel_label) () <br> |
|  MUDA\_GENERIC::cudaStream\_t | [**stream**](classmuda_1_1_launch_core.md#function-stream) () const<br> |








## Public Types Documentation




### typedef NodeParms 

```C++
using muda::ParallelFor::NodeParms =  KernelNodeParms<details::ParallelForCallable<raw_type_t<F> >>;
```




<hr>
## Public Functions Documentation




### function ParallelFor [1/3]

_Calculate grid dim automatically to cover the range, automatially choose the block size to achieve max occupancy._ 
```C++
inline MUDA_HOST muda::ParallelFor::ParallelFor (
    size_t shared_mem_size=0,
    cudaStream_t stream=nullptr
) 
```




```C++
DeviceBuffer<int> buffer(256);
ParallelFor()
    .kernel_name("set_buffer") // optional
    .apply(buffer.size(), 
        [
            buffer = buffer.viewer().name("buffer") // name is optional
        ] __device__(int i) mutable 
        {
            buffer(i) = 1;
        });
```
 


        

<hr>



### function ParallelFor [2/3]

_Calculate grid dim automatically to cover the range, but you need mannally set the block size._ 
```C++
inline MUDA_HOST muda::ParallelFor::ParallelFor (
    int blockDim,
    size_t shared_mem_size=0,
    cudaStream_t stream=nullptr
) 
```




```C++
DeviceBuffer<int> buffer(256);
ParallelFor(64)
    .kernel_name("set_buffer") // optional
    .apply(buffer.size(), 
        [
            buffer = buffer.viewer().name("buffer") // name is optional
        ] __device__(int i) mutable 
        {
            buffer(i) = 1;
        });
```
 


        

<hr>



### function ParallelFor [3/3]

_Use Gride Stride Loop to cover the range, you need mannally set the grid size and block size. Gride Stride Loop: if grid\_dim \* block\_dim &lt; count, there will be a loop in every thread, to process multiple indices._ 
```C++
inline MUDA_HOST muda::ParallelFor::ParallelFor (
    int gridDim,
    int blockDim,
    size_t shared_mem_size=0,
    cudaStream_t stream=nullptr
) 
```




```C++
DeviceBuffer<int> buffer(256);
ParallelFor(2, 64)
    .kernel_name("set_buffer") // optional
    .apply(buffer.size(), 
        [
            buffer = buffer.viewer().name("buffer") // name is optional
        ] __device__(int i) mutable 
        {
            buffer(i) = 1;
        });
```
 


        

<hr>



### function apply [1/2]

```C++
template<typename F, typename UserTag>
MUDA_HOST ParallelFor & muda::ParallelFor::apply (
    int count,
    F && f
) 
```




<hr>



### function apply [2/2]

```C++
template<typename F, typename UserTag>
MUDA_HOST ParallelFor & muda::ParallelFor::apply (
    int count,
    F && f,
    Tag < UserTag >
) 
```




<hr>



### function as\_node\_parms [1/2]

```C++
template<typename F, typename UserTag>
MUDA_HOST MUDA_NODISCARD auto muda::ParallelFor::as_node_parms (
    int count,
    F && f
) 
```




<hr>



### function as\_node\_parms [2/2]

```C++
template<typename F, typename UserTag>
MUDA_HOST MUDA_NODISCARD auto muda::ParallelFor::as_node_parms (
    int count,
    F && f,
    Tag < UserTag >
) 
```




<hr>



### function calculate\_block\_dim 

```C++
template<typename F, typename UserTag>
MUDA_GENERIC int muda::ParallelFor::calculate_block_dim (
    int count
) const
```




<hr>



### function calculate\_grid\_dim [1/2]

```C++
MUDA_GENERIC int muda::ParallelFor::calculate_grid_dim (
    int count
) const
```




<hr>



### function check\_input 

```C++
MUDA_GENERIC void muda::ParallelFor::check_input (
    int count
) const
```




<hr>



### function invoke 

```C++
template<typename F, typename UserTag>
MUDA_HOST void muda::ParallelFor::invoke (
    int count,
    F && f
) 
```




<hr>
## Public Static Functions Documentation




### function calculate\_grid\_dim [2/2]

```C++
static MUDA_GENERIC int muda::ParallelFor::calculate_grid_dim (
    int count,
    int block_dim
) 
```




<hr>



### function round\_up\_blocks 

```C++
static inline MUDA_GENERIC static MUDA_NODISCARD int muda::ParallelFor::round_up_blocks (
    int count,
    int block_dim
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/parallel_for.h`

