

# Class muda::DeviceScan



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceScan**](classmuda_1_1_device_scan.md)








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
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveScan**](#function-exclusivescan-12) (InputIteratorT d\_in, OutputIteratorT d\_out, ScanOpT scan\_op, InitValueT init\_value, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveScan**](#function-exclusivescan-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, ScanOpT scan\_op, InitValueT init\_value, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveScanByKey**](#function-exclusivescanbykey-12) (KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, ScanOpT scan\_op, InitValueT init\_value, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveScanByKey**](#function-exclusivescanbykey-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, ScanOpT scan\_op, InitValueT init\_value, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveSum**](#function-exclusivesum-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveSum**](#function-exclusivesum-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveSumByKey**](#function-exclusivesumbykey-12) (KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**ExclusiveSumByKey**](#function-exclusivesumbykey-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveScan**](#function-inclusivescan-12) (InputIteratorT d\_in, OutputIteratorT d\_out, ScanOpT scan\_op, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveScan**](#function-inclusivescan-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, ScanOpT scan\_op, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveScanByKey**](#function-inclusivescanbykey-12) (KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, ScanOpT scan\_op, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveScanByKey**](#function-inclusivescanbykey-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, ScanOpT scan\_op, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveSum**](#function-inclusivesum-12) (InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveSum**](#function-inclusivesum-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, InputIteratorT d\_in, OutputIteratorT d\_out, int num\_items) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveSumByKey**](#function-inclusivesumbykey-12) (KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |
|  [**DeviceScan**](classmuda_1_1_device_scan.md) & | [**InclusiveSumByKey**](#function-inclusivesumbykey-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeysInputIteratorT d\_keys\_in, ValuesInputIteratorT d\_values\_in, ValuesOutputIteratorT d\_values\_out, int num\_items, EqualityOpT equality\_op=EqualityOpT()) <br> |


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




### function ExclusiveScan [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT, typename ScanOpT, typename InitValueT>
inline DeviceScan & muda::DeviceScan::ExclusiveScan (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    ScanOpT scan_op,
    InitValueT init_value,
    int num_items
) 
```




<hr>



### function ExclusiveScan [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT, typename ScanOpT, typename InitValueT>
inline DeviceScan & muda::DeviceScan::ExclusiveScan (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    ScanOpT scan_op,
    InitValueT init_value,
    int num_items
) 
```




<hr>



### function ExclusiveScanByKey [1/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename ScanOpT, typename InitValueT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::ExclusiveScanByKey (
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    ScanOpT scan_op,
    InitValueT init_value,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function ExclusiveScanByKey [2/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename ScanOpT, typename InitValueT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::ExclusiveScanByKey (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    ScanOpT scan_op,
    InitValueT init_value,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function ExclusiveSum [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceScan & muda::DeviceScan::ExclusiveSum (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function ExclusiveSum [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceScan & muda::DeviceScan::ExclusiveSum (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function ExclusiveSumByKey [1/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::ExclusiveSumByKey (
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function ExclusiveSumByKey [2/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::ExclusiveSumByKey (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function InclusiveScan [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT, typename ScanOpT>
inline DeviceScan & muda::DeviceScan::InclusiveScan (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    ScanOpT scan_op,
    int num_items
) 
```




<hr>



### function InclusiveScan [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT, typename ScanOpT>
inline DeviceScan & muda::DeviceScan::InclusiveScan (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    ScanOpT scan_op,
    int num_items
) 
```




<hr>



### function InclusiveScanByKey [1/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename ScanOpT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::InclusiveScanByKey (
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    ScanOpT scan_op,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function InclusiveScanByKey [2/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename ScanOpT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::InclusiveScanByKey (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    ScanOpT scan_op,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function InclusiveSum [1/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceScan & muda::DeviceScan::InclusiveSum (
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function InclusiveSum [2/2]

```C++
template<typename InputIteratorT, typename OutputIteratorT>
inline DeviceScan & muda::DeviceScan::InclusiveSum (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    InputIteratorT d_in,
    OutputIteratorT d_out,
    int num_items
) 
```




<hr>



### function InclusiveSumByKey [1/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::InclusiveSumByKey (
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>



### function InclusiveSumByKey [2/2]

```C++
template<typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT, typename EqualityOpT>
inline DeviceScan & muda::DeviceScan::InclusiveSumByKey (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeysInputIteratorT d_keys_in,
    ValuesInputIteratorT d_values_in,
    ValuesOutputIteratorT d_values_out,
    int num_items,
    EqualityOpT equality_op=EqualityOpT()
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/cub/device/device_scan.h`

