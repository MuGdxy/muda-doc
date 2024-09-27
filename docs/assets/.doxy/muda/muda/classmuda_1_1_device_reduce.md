

# Class muda::DeviceReduce



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceReduce**](classmuda_1_1_device_reduce.md)








Inherits the following classes: [muda::CubWrapper](classmuda_1_1_cub_wrapper.md)


















## Public Types inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](classmuda_1_1_launch_base.md#typedef-derived_type)  <br> |














## Public Attributes inherited from muda::CubWrapper

See [muda::CubWrapper](classmuda_1_1_cub_wrapper.md)

| Type | Name |
| ---: | :--- |
|  [**Stream**](classmuda_1_1_stream.md) \* | [**m\_muda\_stream**](classmuda_1_1_cub_wrapper.md#variable-m_muda_stream)   = = nullptr<br> |






























































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**ArgMax**](#function-argmax-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**ArgMax**](#function-argmax-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**ArgMin**](#function-argmin-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**ArgMin**](#function-argmin-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Max**](#function-max-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Max**](#function-max-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Min**](#function-min-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Min**](#function-min-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Reduce**](#function-reduce-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items, ReductionOpT reduction\_op, T init) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Reduce**](#function-reduce-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items, ReductionOpT reduction\_op, T init) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**ReduceByKey**](#function-reducebykey-12) (KeysInputIteratorT d\_keys\_in, UniqueOutputIteratorT d\_unique\_out, ValuesInputIteratorT d\_values\_in, AggregatesOutputIteratorT d\_aggregates\_out, NumRunsOutputIteratorT d\_num\_runs\_out, ReductionOpT reduction\_op, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**ReduceByKey**](#function-reducebykey-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeysInputIteratorT d\_keys\_in, UniqueOutputIteratorT d\_unique\_out, ValuesInputIteratorT d\_values\_in, AggregatesOutputIteratorT d\_aggregates\_out, NumRunsOutputIteratorT d\_num\_runs\_out, ReductionOpT reduction\_op, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Sum**](#function-sum-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceReduce**](classmuda_1_1_device_reduce.md) & | [**Sum**](#function-sum-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |


## Public Functions inherited from muda::CubWrapper

See [muda::CubWrapper](classmuda_1_1_cub_wrapper.md)

| Type | Name |
| ---: | :--- |
|   | [**CubWrapper**](classmuda_1_1_cub_wrapper.md#function-cubwrapper) ([**Stream**](classmuda_1_1_stream.md) & stream=Stream::Default()) <br> |
|  void | [**kernel\_name**](classmuda_1_1_cub_wrapper.md#function-kernel_name) (std::string\_view) = delete<br> |


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




























































## Protected Functions inherited from muda::CubWrapper

See [muda::CubWrapper](classmuda_1_1_cub_wrapper.md)

| Type | Name |
| ---: | :--- |
|  std::byte \* | [**prepare\_buffer**](classmuda_1_1_cub_wrapper.md#function-prepare_buffer) (size\_t reqSize) <br> |


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




### function ArgMax [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::ArgMax (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function ArgMax [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::ArgMax (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function ArgMin [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::ArgMin (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function ArgMin [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::ArgMin (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function Max [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::Max (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function Max [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::Max (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function Min [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::Min (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function Min [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::Min (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function Reduce [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT, typename ReductionOpT, typename T>
inline DeviceReduce & muda::DeviceReduce::Reduce (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items,
    ReductionOpT reduction_op,
    T init
) 
```




<hr>



### function Reduce [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT, typename ReductionOpT, typename T>
inline DeviceReduce & muda::DeviceReduce::Reduce (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items,
    ReductionOpT reduction_op,
    T init
) 
```




<hr>



### function ReduceByKey [1/2]

```C++
template<typename KeysInputIteratorT, typename UniqueOutputIteratorT, typename ValuesInputIteratorT, typename AggregatesOutputIteratorT, typename NumRunsOutputIteratorT, typename ReductionOpT>
inline DeviceReduce & muda::DeviceReduce::ReduceByKey (
    KeysInputIteratorT d_keys_in,
    UniqueOutputIteratorT d_unique_out,
    ValuesInputIteratorT d_values_in,
    AggregatesOutputIteratorT d_aggregates_out,
    NumRunsOutputIteratorT d_num_runs_out,
    ReductionOpT reduction_op,
    int num_items
) 
```




<hr>



### function ReduceByKey [2/2]

```C++
template<typename KeysInputIteratorT, typename UniqueOutputIteratorT, typename ValuesInputIteratorT, typename AggregatesOutputIteratorT, typename NumRunsOutputIteratorT, typename ReductionOpT>
inline DeviceReduce & muda::DeviceReduce::ReduceByKey (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeysInputIteratorT d_keys_in,
    UniqueOutputIteratorT d_unique_out,
    ValuesInputIteratorT d_values_in,
    AggregatesOutputIteratorT d_aggregates_out,
    NumRunsOutputIteratorT d_num_runs_out,
    ReductionOpT reduction_op,
    int num_items
) 
```




<hr>



### function Sum [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::Sum (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function Sum [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceReduce & muda::DeviceReduce::Sum (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/cub/device/device_reduce.h`

