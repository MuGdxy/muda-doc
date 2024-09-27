

# Class muda::LaunchBase

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**LaunchBase**](classmuda_1_1_launch_base.md)








Inherits the following classes: [muda::LaunchCore](classmuda_1_1_launch_core.md)


Inherited by the following classes: [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md),  [muda::CubWrapper](classmuda_1_1_cub_wrapper.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](#typedef-derived_type)  <br> |








































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**LaunchBase**](#function-launchbase-22) (::cudaStream\_t stream) <br> |
|  T & | [**callback**](#function-callback) (const std::function&lt; void(::cudaStream\_t, ::cudaError)&gt; & callback) <br> |
|  T & | [**file\_line**](#function-file_line) (std::string\_view file, int line) <br> |
|  T & | [**kernel\_name**](#function-kernel_name) (std::string\_view name) <br> |
|  Next | [**next**](#function-next-12) (Next n) <br> |
|  Next | [**next**](#function-next-22) (Args &&... args) <br> |
|  T & | [**pop\_range**](#function-pop_range) () <br> |
|  T & | [**push\_range**](#function-push_range) (const std::string & name) <br> |
|  T & | [**record**](#function-record-13) (cudaEvent\_t e, int flag=cudaEventRecordDefault) <br> |
|  T & | [**record**](#function-record-23) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  T & | [**record**](#function-record-33) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  T & | [**wait**](#function-wait-14) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|  T & | [**wait**](#function-wait-24) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  T & | [**wait**](#function-wait-34) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  T & | [**wait**](#function-wait-44) () <br> |
|  T & | [**when**](#function-when) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|   | [**~LaunchBase**](#function-launchbase) () <br> |


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






























## Protected Functions

| Type | Name |
| ---: | :--- |
|  T & | [**pop\_kernel\_label**](#function-pop_kernel_label) () <br> |


## Protected Functions inherited from muda::LaunchCore

See [muda::LaunchCore](classmuda_1_1_launch_core.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST void | [**pop\_kernel\_label**](classmuda_1_1_launch_core.md#function-pop_kernel_label) () <br> |
|  MUDA\_GENERIC::cudaStream\_t | [**stream**](classmuda_1_1_launch_core.md#function-stream) () const<br> |






## Public Types Documentation




### typedef derived\_type 

```C++
using muda::LaunchBase< T >::derived_type =  T;
```




<hr>
## Public Functions Documentation




### function LaunchBase [2/2]

```C++
MUDA_GENERIC muda::LaunchBase::LaunchBase (
    ::cudaStream_t stream
) 
```




<hr>



### function callback 

```C++
T & muda::LaunchBase::callback (
    const std::function< void(::cudaStream_t, ::cudaError)> & callback
) 
```




<hr>



### function file\_line 

```C++
T & muda::LaunchBase::file_line (
    std::string_view file,
    int line
) 
```




<hr>



### function kernel\_name 

```C++
T & muda::LaunchBase::kernel_name (
    std::string_view name
) 
```




<hr>



### function next [1/2]

```C++
template<typename Next>
Next muda::LaunchBase::next (
    Next n
) 
```




<hr>



### function next [2/2]

```C++
template<typename Next, typename... Args>
Next muda::LaunchBase::next (
    Args &&... args
) 
```




<hr>



### function pop\_range 

```C++
T & muda::LaunchBase::pop_range () 
```




<hr>



### function push\_range 

```C++
T & muda::LaunchBase::push_range (
    const std::string & name
) 
```




<hr>



### function record [1/3]

```C++
T & muda::LaunchBase::record (
    cudaEvent_t e,
    int flag=cudaEventRecordDefault
) 
```




<hr>



### function record [2/3]

```C++
T & muda::LaunchBase::record (
    ComputeGraphVar < cudaEvent_t > & e,
    const std::vector< ComputeGraphVarBase * > & vars
) 
```




<hr>



### function record [3/3]

```C++
template<typename... ViewT>
T & muda::LaunchBase::record (
    ComputeGraphVar < cudaEvent_t > & e,
    ComputeGraphVar < ViewT > &... vars
) 
```




<hr>



### function wait [1/4]

```C++
T & muda::LaunchBase::wait (
    cudaEvent_t e,
    int flag=cudaEventWaitDefault
) 
```




<hr>



### function wait [2/4]

```C++
T & muda::LaunchBase::wait (
    const ComputeGraphVar < cudaEvent_t > & e,
    const std::vector< ComputeGraphVarBase * > & vars
) 
```




<hr>



### function wait [3/4]

```C++
template<typename... ViewT>
T & muda::LaunchBase::wait (
    const ComputeGraphVar < cudaEvent_t > & e,
    ComputeGraphVar < ViewT > &... vars
) 
```




<hr>



### function wait [4/4]

```C++
T & muda::LaunchBase::wait () 
```




<hr>



### function when 

```C++
T & muda::LaunchBase::when (
    cudaEvent_t e,
    int flag=cudaEventWaitDefault
) 
```




<hr>



### function ~LaunchBase 

```C++
muda::LaunchBase::~LaunchBase () 
```




<hr>
## Protected Functions Documentation




### function pop\_kernel\_label 

```C++
T & muda::LaunchBase::pop_kernel_label () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/launch_base.h`

