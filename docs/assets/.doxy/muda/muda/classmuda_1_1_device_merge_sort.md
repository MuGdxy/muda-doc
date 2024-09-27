

# Class muda::DeviceMergeSort



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md)








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
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortKeys**](#function-sortkeys-12) (KeyIteratorT d\_keys, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortKeys**](#function-sortkeys-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeyIteratorT d\_keys, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortKeysCopy**](#function-sortkeyscopy-12) (KeyInputIteratorT d\_input\_keys, KeyIteratorT d\_output\_keys, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortKeysCopy**](#function-sortkeyscopy-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeyInputIteratorT d\_input\_keys, KeyIteratorT d\_output\_keys, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortPairs**](#function-sortpairs-12) (KeyIteratorT d\_keys, ValueIteratorT d\_items, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortPairs**](#function-sortpairs-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeyIteratorT d\_keys, ValueIteratorT d\_items, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortPairsCopy**](#function-sortpairscopy-12) (KeyInputIteratorT d\_input\_keys, ValueInputIteratorT d\_input\_items, KeyIteratorT d\_output\_keys, ValueIteratorT d\_output\_items, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**SortPairsCopy**](#function-sortpairscopy-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeyInputIteratorT d\_input\_keys, ValueInputIteratorT d\_input\_items, KeyIteratorT d\_output\_keys, ValueIteratorT d\_output\_items, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**StableSortKeys**](#function-stablesortkeys-12) (KeyIteratorT d\_keys, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**StableSortKeys**](#function-stablesortkeys-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeyIteratorT d\_keys, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**StableSortPairs**](#function-stablesortpairs-12) (KeyIteratorT d\_keys, ValueIteratorT d\_items, OffsetT num\_items, CompareOpT compare\_op) <br> |
|  [**DeviceMergeSort**](classmuda_1_1_device_merge_sort.md) & | [**StableSortPairs**](#function-stablesortpairs-22) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, KeyIteratorT d\_keys, ValueIteratorT d\_items, OffsetT num\_items, CompareOpT compare\_op) <br> |


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




### function SortKeys [1/2]

```C++
template<typename KeyIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortKeys (
    KeyIteratorT d_keys,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortKeys [2/2]

```C++
template<typename KeyIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeyIteratorT d_keys,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortKeysCopy [1/2]

```C++
template<typename KeyInputIteratorT, typename KeyIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortKeysCopy (
    KeyInputIteratorT d_input_keys,
    KeyIteratorT d_output_keys,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortKeysCopy [2/2]

```C++
template<typename KeyInputIteratorT, typename KeyIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortKeysCopy (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeyInputIteratorT d_input_keys,
    KeyIteratorT d_output_keys,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortPairs [1/2]

```C++
template<typename KeyIteratorT, typename ValueIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortPairs (
    KeyIteratorT d_keys,
    ValueIteratorT d_items,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortPairs [2/2]

```C++
template<typename KeyIteratorT, typename ValueIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeyIteratorT d_keys,
    ValueIteratorT d_items,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortPairsCopy [1/2]

```C++
template<typename KeyInputIteratorT, typename ValueInputIteratorT, typename KeyIteratorT, typename ValueIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortPairsCopy (
    KeyInputIteratorT d_input_keys,
    ValueInputIteratorT d_input_items,
    KeyIteratorT d_output_keys,
    ValueIteratorT d_output_items,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function SortPairsCopy [2/2]

```C++
template<typename KeyInputIteratorT, typename ValueInputIteratorT, typename KeyIteratorT, typename ValueIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::SortPairsCopy (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeyInputIteratorT d_input_keys,
    ValueInputIteratorT d_input_items,
    KeyIteratorT d_output_keys,
    ValueIteratorT d_output_items,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function StableSortKeys [1/2]

```C++
template<typename KeyIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::StableSortKeys (
    KeyIteratorT d_keys,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function StableSortKeys [2/2]

```C++
template<typename KeyIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::StableSortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeyIteratorT d_keys,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function StableSortPairs [1/2]

```C++
template<typename KeyIteratorT, typename ValueIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::StableSortPairs (
    KeyIteratorT d_keys,
    ValueIteratorT d_items,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>



### function StableSortPairs [2/2]

```C++
template<typename KeyIteratorT, typename ValueIteratorT, typename OffsetT, typename CompareOpT>
inline DeviceMergeSort & muda::DeviceMergeSort::StableSortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    KeyIteratorT d_keys,
    ValueIteratorT d_items,
    OffsetT num_items,
    CompareOpT compare_op
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/cub/device/device_merge_sort.h`

