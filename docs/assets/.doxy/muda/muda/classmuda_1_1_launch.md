

# Class muda::Launch



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Launch**](classmuda_1_1_launch.md)



**A wrapper of raw cuda kernel launch in muda style** _, removing the_`<<<>>>` _usage, for better intellisense support._[More...](#detailed-description)

* `#include <launch.h>`



Inherits the following classes: [muda::LaunchBase](classmuda_1_1_launch_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**KernelNodeParms**](classmuda_1_1_kernel_node_parms.md)&lt; [**details::LaunchCallable**](structmuda_1_1details_1_1_launch_callable.md)&lt; raw\_type\_t&lt; F &gt; &gt; &gt; | [**NodeParms**](#typedef-nodeparms)  <br> |


## Public Types inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](classmuda_1_1_launch_base.md#typedef-derived_type)  <br> |


























































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST | [**Launch**](#function-launch-13) (dim3 gridDim, dim3 blockDim, size\_t sharedMemSize=0, cudaStream\_t stream=nullptr) <br> |
|  MUDA\_HOST | [**Launch**](#function-launch-23) (int gridDim=1, int blockDim=1, size\_t sharedMemSize=0, cudaStream\_t stream=nullptr) <br> |
|  MUDA\_HOST | [**Launch**](#function-launch-33) (dim3 blockDim, size\_t sharedMemSize=0, cudaStream\_t stream=nullptr) <br> |
|  MUDA\_HOST [**Launch**](classmuda_1_1_launch.md) & | [**apply**](#function-apply-14) (F && f) <br> |
|  MUDA\_HOST [**Launch**](classmuda_1_1_launch.md) & | [**apply**](#function-apply-24) (F && f, [**Tag**](structmuda_1_1_tag.md)&lt; UserTag &gt;) <br> |
|  MUDA\_HOST [**Launch**](classmuda_1_1_launch.md) & | [**apply**](#function-apply-34) (const dim3 & active\_dim, F && f) <br> |
|  MUDA\_HOST [**Launch**](classmuda_1_1_launch.md) & | [**apply**](#function-apply-44) (const dim3 & active\_dim, F && f, [**Tag**](structmuda_1_1_tag.md)&lt; UserTag &gt;) <br> |
|  MUDA\_HOST MUDA\_NODISCARD auto | [**as\_node\_parms**](#function-as_node_parms-14) (F && f) <br> |
|  MUDA\_HOST MUDA\_NODISCARD auto | [**as\_node\_parms**](#function-as_node_parms-24) (F && f, [**Tag**](structmuda_1_1_tag.md)&lt; UserTag &gt;) <br> |
|  MUDA\_HOST MUDA\_NODISCARD auto | [**as\_node\_parms**](#function-as_node_parms-34) (const dim3 & active\_dim, F && f) <br> |
|  MUDA\_HOST MUDA\_NODISCARD auto | [**as\_node\_parms**](#function-as_node_parms-44) (const dim3 & active\_dim, F && f, [**Tag**](structmuda_1_1_tag.md)&lt; UserTag &gt;) <br> |


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








# Detailed Description


A raw cuda kernel define and launch: 
```C++
__global__ void cuda_kernel() {}

int main()
{
    cuda_kernel<<<4,64>>>();
}
```



The muda style kernel launch: 
```C++
// muda kernel launch
Launch(4,64)
    .kernel_name("kernel_name") // optional
    .apply([]__device__(){}); // kernel body
```



A more complicated but more convincing example, to show why using muda style kernel launch is better than raw cuda kernel launch. 
```C++
DeviceBuffer3D<float> volume{10,10,10};
Launch(dim3{8,8,8}) // blockDim
    .kernel_name("write_volume") // optional, for better debug info
    .apply(volume.extent(), 
        [
            volume = volume.viewer().name("volume") // name is optional, for better debug info
        ] __device__(int3 xyz) mutable
        {
            volume(xyz) = 1.0f;
        });
```





**See also:** [**device\_buffer\_3d.h**](device__buffer__3d_8h.md) [**parallel\_for.h**](parallel__for_8h.md) 



    
## Public Types Documentation




### typedef NodeParms 

```C++
using muda::Launch::NodeParms =  KernelNodeParms<details::LaunchCallable<raw_type_t<F> >>;
```




<hr>
## Public Functions Documentation




### function Launch [1/3]

```C++
inline MUDA_HOST muda::Launch::Launch (
    dim3 gridDim,
    dim3 blockDim,
    size_t sharedMemSize=0,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function Launch [2/3]

```C++
inline MUDA_HOST muda::Launch::Launch (
    int gridDim=1,
    int blockDim=1,
    size_t sharedMemSize=0,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function Launch [3/3]

```C++
inline MUDA_HOST muda::Launch::Launch (
    dim3 blockDim,
    size_t sharedMemSize=0,
    cudaStream_t stream=nullptr
) 
```




<hr>



### function apply [1/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST Launch & muda::Launch::apply (
    F && f
) 
```




<hr>



### function apply [2/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST Launch & muda::Launch::apply (
    F && f,
    Tag < UserTag >
) 
```




<hr>



### function apply [3/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST Launch & muda::Launch::apply (
    const dim3 & active_dim,
    F && f
) 
```




<hr>



### function apply [4/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST Launch & muda::Launch::apply (
    const dim3 & active_dim,
    F && f,
    Tag < UserTag >
) 
```




<hr>



### function as\_node\_parms [1/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST MUDA_NODISCARD auto muda::Launch::as_node_parms (
    F && f
) 
```




<hr>



### function as\_node\_parms [2/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST MUDA_NODISCARD auto muda::Launch::as_node_parms (
    F && f,
    Tag < UserTag >
) 
```




<hr>



### function as\_node\_parms [3/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST MUDA_NODISCARD auto muda::Launch::as_node_parms (
    const dim3 & active_dim,
    F && f
) 
```




<hr>



### function as\_node\_parms [4/4]

```C++
template<typename F, typename UserTag>
MUDA_HOST MUDA_NODISCARD auto muda::Launch::as_node_parms (
    const dim3 & active_dim,
    F && f,
    Tag < UserTag >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/launch.h`

