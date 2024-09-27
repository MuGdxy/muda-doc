

# Class muda::LaunchCore



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**LaunchCore**](classmuda_1_1_launch_core.md)










Inherited by the following classes: [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md),  [muda::LaunchBase](classmuda_1_1_launch_base.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**LaunchCore**](#function-launchcore) (::cudaStream\_t stream) <br> |
|  void | [**callback**](#function-callback) (const std::function&lt; void(::cudaStream\_t, ::cudaError)&gt; & callback) <br> |
|  void | [**init\_stream**](#function-init_stream) (::cudaStream\_t s) <br> |
|  void | [**pop\_range**](#function-pop_range) () <br> |
|  void | [**push\_range**](#function-push_range) (const std::string & name) <br> |
|  void | [**record**](#function-record-13) (cudaEvent\_t e, int flag=cudaEventRecordDefault) <br> |
|  void | [**record**](#function-record-23) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  void | [**record**](#function-record-33) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  void | [**wait**](#function-wait-14) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|  void | [**wait**](#function-wait-24) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, const std::vector&lt; [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; & vars) <br> |
|  void | [**wait**](#function-wait-34) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; cudaEvent\_t &gt; & e, [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; ViewT &gt; &... vars) <br> |
|  void | [**wait**](#function-wait-44) () <br> |
|  void | [**when**](#function-when) (cudaEvent\_t e, int flag=cudaEventWaitDefault) <br> |
|   | [**~LaunchCore**](#function-launchcore) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**file\_line**](#function-file_line) (std::string\_view file, int line) <br> |
|  void | [**kernel\_name**](#function-kernel_name) (std::string\_view name) <br> |
|  void | [**wait\_device**](#function-wait_device) () <br> |
|  void | [**wait\_event**](#function-wait_event) (cudaEvent\_t event) <br> |
|  void | [**wait\_stream**](#function-wait_stream) (::cudaStream\_t stream) <br> |


## Protected Types

| Type | Name |
| ---: | :--- |
| typedef std::shared\_ptr&lt; T &gt; | [**S**](#typedef-s)  <br> |




## Protected Attributes

| Type | Name |
| ---: | :--- |
|  ::cudaStream\_t | [**m\_stream**](#variable-m_stream)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST void | [**pop\_kernel\_label**](#function-pop_kernel_label) () <br> |
|  MUDA\_GENERIC::cudaStream\_t | [**stream**](#function-stream) () const<br> |




## Public Functions Documentation




### function LaunchCore 

```C++
MUDA_GENERIC muda::LaunchCore::LaunchCore (
    ::cudaStream_t stream
) 
```




<hr>



### function callback 

```C++
void muda::LaunchCore::callback (
    const std::function< void(::cudaStream_t, ::cudaError)> & callback
) 
```




<hr>



### function init\_stream 

```C++
inline void muda::LaunchCore::init_stream (
    ::cudaStream_t s
) 
```




<hr>



### function pop\_range 

```C++
void muda::LaunchCore::pop_range () 
```




<hr>



### function push\_range 

```C++
void muda::LaunchCore::push_range (
    const std::string & name
) 
```




<hr>



### function record [1/3]

```C++
void muda::LaunchCore::record (
    cudaEvent_t e,
    int flag=cudaEventRecordDefault
) 
```




<hr>



### function record [2/3]

```C++
void muda::LaunchCore::record (
    ComputeGraphVar < cudaEvent_t > & e,
    const std::vector< ComputeGraphVarBase * > & vars
) 
```




<hr>



### function record [3/3]

```C++
template<typename... ViewT>
void muda::LaunchCore::record (
    ComputeGraphVar < cudaEvent_t > & e,
    ComputeGraphVar < ViewT > &... vars
) 
```




<hr>



### function wait [1/4]

```C++
void muda::LaunchCore::wait (
    cudaEvent_t e,
    int flag=cudaEventWaitDefault
) 
```




<hr>



### function wait [2/4]

```C++
void muda::LaunchCore::wait (
    const ComputeGraphVar < cudaEvent_t > & e,
    const std::vector< ComputeGraphVarBase * > & vars
) 
```




<hr>



### function wait [3/4]

```C++
template<typename... ViewT>
void muda::LaunchCore::wait (
    const ComputeGraphVar < cudaEvent_t > & e,
    ComputeGraphVar < ViewT > &... vars
) 
```




<hr>



### function wait [4/4]

```C++
void muda::LaunchCore::wait () 
```




<hr>



### function when 

```C++
void muda::LaunchCore::when (
    cudaEvent_t e,
    int flag=cudaEventWaitDefault
) 
```




<hr>



### function ~LaunchCore 

```C++
muda::LaunchCore::~LaunchCore () 
```




<hr>
## Public Static Functions Documentation




### function file\_line 

```C++
static void muda::LaunchCore::file_line (
    std::string_view file,
    int line
) 
```




<hr>



### function kernel\_name 

```C++
static void muda::LaunchCore::kernel_name (
    std::string_view name
) 
```




<hr>



### function wait\_device 

```C++
static void muda::LaunchCore::wait_device () 
```




<hr>



### function wait\_event 

```C++
static void muda::LaunchCore::wait_event (
    cudaEvent_t event
) 
```




<hr>



### function wait\_stream 

```C++
static void muda::LaunchCore::wait_stream (
    ::cudaStream_t stream
) 
```




<hr>
## Protected Types Documentation




### typedef S 

```C++
using muda::LaunchCore::S =  std::shared_ptr<T>;
```




<hr>
## Protected Attributes Documentation




### variable m\_stream 

```C++
::cudaStream_t muda::LaunchCore::m_stream;
```




<hr>
## Protected Functions Documentation




### function pop\_kernel\_label 

```C++
MUDA_HOST void muda::LaunchCore::pop_kernel_label () 
```




<hr>



### function stream 

```C++
inline MUDA_GENERIC::cudaStream_t muda::LaunchCore::stream () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/launch_base.h`

