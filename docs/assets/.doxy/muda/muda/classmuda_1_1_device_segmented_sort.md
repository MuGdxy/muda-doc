

# Class muda::DeviceSegmentedSort



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md)








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
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeys**](#function-sortkeys-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeys**](#function-sortkeys-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeys**](#function-sortkeys-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeys**](#function-sortkeys-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortKeysDescending**](#function-sortkeysdescending-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairs**](#function-sortpairs-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairs**](#function-sortpairs-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairs**](#function-sortpairs-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairs**](#function-sortpairs-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**SortPairsDescending**](#function-sortpairsdescending-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeys**](#function-stablesortkeys-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeys**](#function-stablesortkeys-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeys**](#function-stablesortkeys-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeys**](#function-stablesortkeys-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeysDescending**](#function-stablesortkeysdescending-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeysDescending**](#function-stablesortkeysdescending-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeysDescending**](#function-stablesortkeysdescending-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortKeysDescending**](#function-stablesortkeysdescending-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairs**](#function-stablesortpairs-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairs**](#function-stablesortpairs-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairs**](#function-stablesortpairs-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairs**](#function-stablesortpairs-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairsDescending**](#function-stablesortpairsdescending-14) (const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairsDescending**](#function-stablesortpairsdescending-24) (cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairsDescending**](#function-stablesortpairsdescending-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, const KeyT \* d\_keys\_in, KeyT \* d\_keys\_out, const ValueT \* d\_values\_in, ValueT \* d\_values\_out, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |
|  [**DeviceSegmentedSort**](classmuda_1_1_device_segmented_sort.md) & | [**StableSortPairsDescending**](#function-stablesortpairsdescending-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, cub::DoubleBuffer&lt; KeyT &gt; & d\_keys, cub::DoubleBuffer&lt; ValueT &gt; & d\_values, int num\_items, int num\_segments, BeginOffsetIteratorT d\_begin\_offsets, EndOffsetIteratorT d\_end\_offsets) <br> |


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
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeys (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeys [2/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeys (
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeys [3/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeys [4/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeysDescending [1/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeysDescending (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeysDescending [2/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeysDescending (
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeysDescending [3/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeysDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortKeysDescending [4/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortKeysDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairs [1/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairs (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairs [2/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairs (
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairs [3/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairs [4/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairsDescending [1/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairsDescending (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairsDescending [2/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairsDescending (
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairsDescending [3/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairsDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function SortPairsDescending [4/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::SortPairsDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeys [1/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeys (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeys [2/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeys (
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeys [3/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeys [4/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeys (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeysDescending [1/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeysDescending (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeysDescending [2/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeysDescending (
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeysDescending [3/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeysDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortKeysDescending [4/4]

```C++
template<typename KeyT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortKeysDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairs [1/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairs (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairs [2/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairs (
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairs [3/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairs [4/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairs (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairsDescending [1/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairsDescending (
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairsDescending [2/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairsDescending (
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairsDescending [3/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairsDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    const KeyT * d_keys_in,
    KeyT * d_keys_out,
    const ValueT * d_values_in,
    ValueT * d_values_out,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>



### function StableSortPairsDescending [4/4]

```C++
template<typename KeyT, typename ValueT, typename BeginOffsetIteratorT, typename EndOffsetIteratorT>
inline DeviceSegmentedSort & muda::DeviceSegmentedSort::StableSortPairsDescending (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    cub::DoubleBuffer< KeyT > & d_keys,
    cub::DoubleBuffer< ValueT > & d_values,
    int num_items,
    int num_segments,
    BeginOffsetIteratorT d_begin_offsets,
    EndOffsetIteratorT d_end_offsets
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/cub/device/device_segmented_sort.h`

