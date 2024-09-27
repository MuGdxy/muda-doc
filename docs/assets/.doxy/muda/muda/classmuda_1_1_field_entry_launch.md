

# Class muda::FieldEntryLaunch



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldEntryLaunch**](classmuda_1_1_field_entry_launch.md)








Inherits the following classes: [muda::LaunchBase](classmuda_1_1_launch_base.md)
















## Public Types inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](classmuda_1_1_launch_base.md#typedef-derived_type)  <br> |


























































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**FieldEntryLaunch**](#function-fieldentrylaunch) (cudaStream\_t stream=nullptr) <br> |
|  MUDA\_HOST [**FieldEntryLaunch**](classmuda_1_1_field_entry_launch.md) & | [**copy**](#function-copy-13) ([**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, DstLayout, M, N &gt; dst, [**CFieldEntryView**](classmuda_1_1_c_field_entry_view.md)&lt; T, SrcLayout, M, N &gt; src) <br> |
|  MUDA\_HOST [**FieldEntryLaunch**](classmuda_1_1_field_entry_launch.md) & | [**copy**](#function-copy-23) ([**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; typename [**CFieldEntryView**](classmuda_1_1_c_field_entry_view.md)&lt; T, SrcLayout, M, N &gt;::ElementType &gt; dst, [**CFieldEntryView**](classmuda_1_1_c_field_entry_view.md)&lt; T, SrcLayout, M, N &gt; src) <br> |
|  MUDA\_HOST [**FieldEntryLaunch**](classmuda_1_1_field_entry_launch.md) & | [**copy**](#function-copy-33) ([**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, DstLayout, M, N &gt; dst, [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; typename [**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, DstLayout, M, N &gt;::ElementType &gt; src) <br> |
|  MUDA\_HOST [**FieldEntryLaunch**](classmuda_1_1_field_entry_launch.md) & | [**fill**](#function-fill) ([**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, DstLayout, M, N &gt; dst, const typename [**FieldEntryView**](classmuda_1_1_field_entry_view.md)&lt; T, DstLayout, M, N &gt;::ElementType & value) <br> |


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




### function FieldEntryLaunch 

```C++
inline MUDA_GENERIC muda::FieldEntryLaunch::FieldEntryLaunch (
    cudaStream_t stream=nullptr
) 
```




<hr>



### function copy [1/3]

```C++
template<typename T, FieldEntryLayout DstLayout, FieldEntryLayout SrcLayout, int M, int N>
MUDA_HOST FieldEntryLaunch & muda::FieldEntryLaunch::copy (
    FieldEntryView < T, DstLayout, M, N > dst,
    CFieldEntryView < T, SrcLayout, M, N > src
) 
```




<hr>



### function copy [2/3]

```C++
template<typename T, FieldEntryLayout SrcLayout, int M, int N>
MUDA_HOST FieldEntryLaunch & muda::FieldEntryLaunch::copy (
    BufferView < typename CFieldEntryView < T, SrcLayout, M, N >::ElementType > dst,
    CFieldEntryView < T, SrcLayout, M, N > src
) 
```




<hr>



### function copy [3/3]

```C++
template<typename T, FieldEntryLayout DstLayout, int M, int N>
MUDA_HOST FieldEntryLaunch & muda::FieldEntryLaunch::copy (
    FieldEntryView < T, DstLayout, M, N > dst,
    CBufferView < typename FieldEntryView < T, DstLayout, M, N >::ElementType > src
) 
```




<hr>



### function fill 

```C++
template<typename T, FieldEntryLayout DstLayout, int M, int N>
MUDA_HOST FieldEntryLaunch & muda::FieldEntryLaunch::fill (
    FieldEntryView < T, DstLayout, M, N > dst,
    const typename FieldEntryView < T, DstLayout, M, N >::ElementType & value
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_entry_launch.h`

