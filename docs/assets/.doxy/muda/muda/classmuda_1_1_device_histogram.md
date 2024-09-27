

# Class muda::DeviceHistogram



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DeviceHistogram**](classmuda_1_1_device_histogram.md)








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
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramEven**](#function-histogrameven-14) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_samples) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramEven**](#function-histogrameven-24) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_row\_samples, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramEven**](#function-histogrameven-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_samples) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramEven**](#function-histogrameven-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_row\_samples, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramRange**](#function-histogramrange-14) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_samples) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramRange**](#function-histogramrange-24) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_row\_samples, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramRange**](#function-histogramrange-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_samples) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**HistogramRange**](#function-histogramrange-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_row\_samples, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramEven**](#function-multihistogrameven-14) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_pixels) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramEven**](#function-multihistogrameven-24) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_row\_pixels, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramEven**](#function-multihistogrameven-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_pixels) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramEven**](#function-multihistogrameven-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT lower\_level, LevelT upper\_level, OffsetT num\_row\_pixels, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramRange**](#function-multihistogramrange-14) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_pixels) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramRange**](#function-multihistogramrange-24) (SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_row\_pixels, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramRange**](#function-multihistogramrange-34) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_pixels) <br> |
|  [**DeviceHistogram**](classmuda_1_1_device_histogram.md) & | [**MultiHistogramRange**](#function-multihistogramrange-44) (void \* d\_temp\_storage, size\_t & temp\_storage\_bytes, SampleIteratorT d\_samples, CounterT \* d\_histogram, int num\_levels, LevelT \* d\_levels, OffsetT num\_row\_pixels, OffsetT num\_rows, size\_t row\_stride\_bytes) <br> |


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




### function HistogramEven [1/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramEven (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_samples
) 
```




<hr>



### function HistogramEven [2/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramEven (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_row_samples,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function HistogramEven [3/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramEven (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_samples
) 
```




<hr>



### function HistogramEven [4/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramEven (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_row_samples,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function HistogramRange [1/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramRange (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_samples
) 
```




<hr>



### function HistogramRange [2/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramRange (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_row_samples,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function HistogramRange [3/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramRange (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_samples
) 
```




<hr>



### function HistogramRange [4/4]

```C++
template<typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::HistogramRange (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_row_samples,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function MultiHistogramEven [1/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramEven (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_pixels
) 
```




<hr>



### function MultiHistogramEven [2/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramEven (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_row_pixels,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function MultiHistogramEven [3/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramEven (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_pixels
) 
```




<hr>



### function MultiHistogramEven [4/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramEven (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT lower_level,
    LevelT upper_level,
    OffsetT num_row_pixels,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function MultiHistogramRange [1/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramRange (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_pixels
) 
```




<hr>



### function MultiHistogramRange [2/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramRange (
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_row_pixels,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>



### function MultiHistogramRange [3/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramRange (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_pixels
) 
```




<hr>



### function MultiHistogramRange [4/4]

```C++
template<int NUM_CHANNELS, int NUM_ACTIVE_CHANNELS, typename SampleIteratorT, typename CounterT, typename LevelT, typename OffsetT>
inline DeviceHistogram & muda::DeviceHistogram::MultiHistogramRange (
    void * d_temp_storage,
    size_t & temp_storage_bytes,
    SampleIteratorT d_samples,
    CounterT * d_histogram,
    int num_levels,
    LevelT * d_levels,
    OffsetT num_row_pixels,
    OffsetT num_rows,
    size_t row_stride_bytes
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/cub/device/device_histogram.h`

