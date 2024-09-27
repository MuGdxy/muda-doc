

# Class muda::DeviceSegmentedRadixSort



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md)








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
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeys**](#function-sortkeys-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeys**](#function-sortkeys-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeys**](#function-sortkeys-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeys**](#function-sortkeys-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairs**](#function-sortpairs-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairs**](#function-sortpairs-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairs**](#function-sortpairs-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairs**](#function-sortpairs-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |
|  [**DeviceSegmentedRadixSort**](classmuda_1_1_device_segmented_radix_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets, int begin\_bit, int end\_bit) <br> |


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




### function SortKeys [1/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeys (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeys [2/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeys (
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeys [3/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeys [4/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeysDescending [1/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeysDescending (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeysDescending [2/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeysDescending (
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeysDescending [3/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeysDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortKeysDescending [4/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortKeysDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairs [1/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairs (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairs [2/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairs (
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairs [3/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairs [4/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairsDescending [1/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairsDescending (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairsDescending [2/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairsDescending (
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairsDescending [3/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairsDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>



### function SortPairsDescending [4/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedRadixSort & muda::DeviceSegmentedRadixSort::SortPairsDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets,
    int begin_bit,
    int end_bit
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/cub/device/device_segmented_radix_sort.h`

