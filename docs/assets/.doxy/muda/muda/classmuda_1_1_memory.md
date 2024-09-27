

# Class muda::Memory



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Memory**](classmuda_1_1_memory.md)








Inherits the following classes: [muda::LaunchBase](classmuda_1_1_launch_base.md)
















## Public Types inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](classmuda_1_1_launch_base.md#typedef-derived_type)  <br> |


























































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST | [**Memory**](#function-memory) (cudaStream\_t stream=nullptr) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**alloc**](#function-alloc-13) (T \*\* ptr, size\_t byte\_size, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**alloc**](#function-alloc-23) (T \*\* ptr, size\_t \* pitch, size\_t width\_bytes, size\_t height, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**alloc**](#function-alloc-33) (cudaPitchedPtr \* pitched\_ptr, const cudaExtent & extent, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**alloc\_1d**](#function-alloc_1d) (T \*\* ptr, size\_t byte\_size, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**alloc\_2d**](#function-alloc_2d) (T \*\* ptr, size\_t \* pitch, size\_t width\_bytes, size\_t height, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**alloc\_3d**](#function-alloc_3d) (cudaPitchedPtr \* pitched\_ptr, const cudaExtent & extent, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**copy**](#function-copy-13) (void \* dst, const void \* src, size\_t byte\_size, cudaMemcpyKind kind) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**copy**](#function-copy-23) (void \* dst, size\_t dst\_pitch, const void \* src, size\_t src\_pitch, size\_t width\_bytes, size\_t height, cudaMemcpyKind kind) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**copy**](#function-copy-33) (const cudaMemcpy3DParms & parms) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**download**](#function-download-13) (void \* dst, const void \* src, size\_t byte\_size) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**download**](#function-download-23) (void \* dst, size\_t dst\_pitch, const void \* src, size\_t src\_pitch, size\_t width\_bytes, size\_t height) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**download**](#function-download-33) (cudaMemcpy3DParms parms) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**free**](#function-free-12) (void \* ptr, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**free**](#function-free-22) (cudaPitchedPtr pitched\_ptr, bool async=DEFAULT\_ASYNC\_ALLOC\_FREE) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**set**](#function-set-13) (void \* data, size\_t byte\_size, char value=0) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**set**](#function-set-23) (void \* data, size\_t pitch, size\_t width\_bytes, size\_t height, char value=0) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**set**](#function-set-33) (cudaPitchedPtr pitched\_ptr, cudaExtent extent, char value=0) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**transfer**](#function-transfer-13) (void \* dst, const void \* src, size\_t byte\_size) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**transfer**](#function-transfer-23) (void \* dst, size\_t dst\_pitch, const void \* src, size\_t src\_pitch, size\_t width\_bytes, size\_t height) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**transfer**](#function-transfer-33) (cudaMemcpy3DParms parms) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**upload**](#function-upload-13) (void \* dst, const void \* src, size\_t byte\_size) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**upload**](#function-upload-23) (void \* dst, size\_t dst\_pitch, const void \* src, size\_t src\_pitch, size\_t width\_bytes, size\_t height) <br> |
|  MUDA\_HOST [**Memory**](classmuda_1_1_memory.md) & | [**upload**](#function-upload-33) (cudaMemcpy3DParms parms) <br> |


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








## Public Functions Documentation




### function Memory 

```C++
inline MUDA_HOST muda::Memory::Memory (
    cudaStream_t stream=nullptr
) 
```




<hr>



### function alloc [1/3]

```C++
template<typename T>
MUDA_HOST Memory & muda::Memory::alloc (
    T ** ptr,
    size_t byte_size,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function alloc [2/3]

```C++
template<typename T>
MUDA_HOST Memory & muda::Memory::alloc (
    T ** ptr,
    size_t * pitch,
    size_t width_bytes,
    size_t height,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function alloc [3/3]

```C++
MUDA_HOST Memory & muda::Memory::alloc (
    cudaPitchedPtr * pitched_ptr,
    const cudaExtent & extent,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function alloc\_1d 

```C++
template<typename T>
MUDA_HOST Memory & muda::Memory::alloc_1d (
    T ** ptr,
    size_t byte_size,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function alloc\_2d 

```C++
template<typename T>
MUDA_HOST Memory & muda::Memory::alloc_2d (
    T ** ptr,
    size_t * pitch,
    size_t width_bytes,
    size_t height,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function alloc\_3d 

```C++
MUDA_HOST Memory & muda::Memory::alloc_3d (
    cudaPitchedPtr * pitched_ptr,
    const cudaExtent & extent,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function copy [1/3]

```C++
MUDA_HOST Memory & muda::Memory::copy (
    void * dst,
    const void * src,
    size_t byte_size,
    cudaMemcpyKind kind
) 
```




<hr>



### function copy [2/3]

```C++
MUDA_HOST Memory & muda::Memory::copy (
    void * dst,
    size_t dst_pitch,
    const void * src,
    size_t src_pitch,
    size_t width_bytes,
    size_t height,
    cudaMemcpyKind kind
) 
```




<hr>



### function copy [3/3]

```C++
MUDA_HOST Memory & muda::Memory::copy (
    const cudaMemcpy3DParms & parms
) 
```




<hr>



### function download [1/3]

```C++
MUDA_HOST Memory & muda::Memory::download (
    void * dst,
    const void * src,
    size_t byte_size
) 
```




<hr>



### function download [2/3]

```C++
MUDA_HOST Memory & muda::Memory::download (
    void * dst,
    size_t dst_pitch,
    const void * src,
    size_t src_pitch,
    size_t width_bytes,
    size_t height
) 
```




<hr>



### function download [3/3]

```C++
MUDA_HOST Memory & muda::Memory::download (
    cudaMemcpy3DParms parms
) 
```




<hr>



### function free [1/2]

```C++
MUDA_HOST Memory & muda::Memory::free (
    void * ptr,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function free [2/2]

```C++
MUDA_HOST Memory & muda::Memory::free (
    cudaPitchedPtr pitched_ptr,
    bool async=DEFAULT_ASYNC_ALLOC_FREE
) 
```




<hr>



### function set [1/3]

```C++
MUDA_HOST Memory & muda::Memory::set (
    void * data,
    size_t byte_size,
    char value=0
) 
```




<hr>



### function set [2/3]

```C++
MUDA_HOST Memory & muda::Memory::set (
    void * data,
    size_t pitch,
    size_t width_bytes,
    size_t height,
    char value=0
) 
```




<hr>



### function set [3/3]

```C++
MUDA_HOST Memory & muda::Memory::set (
    cudaPitchedPtr pitched_ptr,
    cudaExtent extent,
    char value=0
) 
```




<hr>



### function transfer [1/3]

```C++
MUDA_HOST Memory & muda::Memory::transfer (
    void * dst,
    const void * src,
    size_t byte_size
) 
```




<hr>



### function transfer [2/3]

```C++
MUDA_HOST Memory & muda::Memory::transfer (
    void * dst,
    size_t dst_pitch,
    const void * src,
    size_t src_pitch,
    size_t width_bytes,
    size_t height
) 
```




<hr>



### function transfer [3/3]

```C++
MUDA_HOST Memory & muda::Memory::transfer (
    cudaMemcpy3DParms parms
) 
```




<hr>



### function upload [1/3]

```C++
MUDA_HOST Memory & muda::Memory::upload (
    void * dst,
    const void * src,
    size_t byte_size
) 
```




<hr>



### function upload [2/3]

```C++
MUDA_HOST Memory & muda::Memory::upload (
    void * dst,
    size_t dst_pitch,
    const void * src,
    size_t src_pitch,
    size_t width_bytes,
    size_t height
) 
```




<hr>



### function upload [3/3]

```C++
MUDA_HOST Memory & muda::Memory::upload (
    cudaMemcpy3DParms parms
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/memory.h`

