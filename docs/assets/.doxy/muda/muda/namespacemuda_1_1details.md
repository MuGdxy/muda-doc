

# Namespace muda::details



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**buffer**](namespacemuda_1_1details_1_1buffer.md) <br> |
| namespace | [**eigen**](namespacemuda_1_1details_1_1eigen.md) <br> |
| namespace | [**field**](namespacemuda_1_1details_1_1field.md) <br> |
| namespace | [**stream**](namespacemuda_1_1details_1_1stream.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**ComputeGraphAccessor**](classmuda_1_1details_1_1_compute_graph_accessor.md) <br> |
| class | [**HostDeviceStringCache**](classmuda_1_1details_1_1_host_device_string_cache.md) <br> |
| struct | [**LaunchCallable**](structmuda_1_1details_1_1_launch_callable.md) &lt;typename F&gt;<br> |
| class | [**LaunchInfoCache**](classmuda_1_1details_1_1_launch_info_cache.md) <br> |
| class | [**LocalVarId**](classmuda_1_1details_1_1_local_var_id.md) <br> |
| class | [**LocalVarInfo**](classmuda_1_1details_1_1_local_var_info.md) <br> |
| class | [**LoggerMetaData**](classmuda_1_1details_1_1_logger_meta_data.md) <br> |
| class | [**LoggerOffset**](classmuda_1_1details_1_1_logger_offset.md) <br> |
| class | [**MatrixFormatConverter**](classmuda_1_1details_1_1_matrix_format_converter.md) &lt;typename T, N&gt;<br> |
| class | [**MatrixFormatConverter&lt; T, 1 &gt;**](classmuda_1_1details_1_1_matrix_format_converter_3_01_t_00_011_01_4.md) &lt;typename T&gt;<br> |
| class | [**MatrixFormatConverterBase**](classmuda_1_1details_1_1_matrix_format_converter_base.md) <br> |
| class | [**MatrixFormatConverterType**](classmuda_1_1details_1_1_matrix_format_converter_type.md) <br> |
| class | [**ParallelForCallable**](classmuda_1_1details_1_1_parallel_for_callable.md) &lt;typename F&gt;<br> |
| struct | [**SoACopyMap**](structmuda_1_1details_1_1_so_a_copy_map.md) <br> |
| class | [**StringPointer**](classmuda_1_1details_1_1_string_pointer.md) <br> |
| class | [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md) &lt;typename T&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**TempBuffer**](classmuda_1_1details_1_1_temp_buffer.md)&lt; std::byte &gt; | [**ByteTempBuffer**](#typedef-bytetempbuffer)  <br> |
| typedef thrust::detail::vector\_base&lt; T, Alloc &gt; | [**vector\_base**](#typedef-vector_base)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST void CUDARTAPI | [**delete\_function\_object**](#function-delete_function_object) (void \* userdata) <br> |
|  MUDA\_HOST void CUDARTAPI | [**generic\_host\_call**](#function-generic_host_call) (void \* userdata) <br> |
|  MUDA\_GLOBAL void | [**generic\_kernel**](#function-generic_kernel) ([**LaunchCallable**](structmuda_1_1details_1_1_launch_callable.md)&lt; F &gt; f) <br> |
|  MUDA\_GLOBAL void | [**generic\_kernel\_with\_range**](#function-generic_kernel_with_range) ([**LaunchCallable**](structmuda_1_1details_1_1_launch_callable.md)&lt; F &gt; f) <br> |
|  MUDA\_GLOBAL void | [**grid\_stride\_loop\_kernel**](#function-grid_stride_loop_kernel) ([**ParallelForCallable**](classmuda_1_1details_1_1_parallel_for_callable.md)&lt; F &gt; f) <br> |
|  MUDA\_GLOBAL void | [**parallel\_for\_kernel**](#function-parallel_for_kernel) ([**ParallelForCallable**](classmuda_1_1details_1_1_parallel_for_callable.md)&lt; F &gt; f) <br> |
|  void | [**stream\_error\_callback**](#function-stream_error_callback) (cudaStream\_t stream, cudaError error, void \* userdata) <br> |




























## Public Types Documentation




### typedef ByteTempBuffer 

```C++
using muda::details::ByteTempBuffer = typedef TempBuffer<std::byte>;
```




<hr>



### typedef vector\_base 

```C++
using muda::details::vector_base = typedef thrust::detail::vector_base<T, Alloc>;
```




<hr>
## Public Functions Documentation




### function delete\_function\_object 

```C++
template<typename F, typename UserTag>
MUDA_HOST void CUDARTAPI muda::details::delete_function_object (
    void * userdata
) 
```




<hr>



### function generic\_host\_call 

```C++
template<typename F, typename UserTag>
MUDA_HOST void CUDARTAPI muda::details::generic_host_call (
    void * userdata
) 
```




<hr>



### function generic\_kernel 

```C++
template<typename F, typename UserTag>
MUDA_GLOBAL void muda::details::generic_kernel (
    LaunchCallable < F > f
) 
```




<hr>



### function generic\_kernel\_with\_range 

```C++
template<typename F, typename UserTag>
MUDA_GLOBAL void muda::details::generic_kernel_with_range (
    LaunchCallable < F > f
) 
```




<hr>



### function grid\_stride\_loop\_kernel 

```C++
template<typename F, typename UserTag>
MUDA_GLOBAL void muda::details::grid_stride_loop_kernel (
    ParallelForCallable < F > f
) 
```




<hr>



### function parallel\_for\_kernel 

```C++
template<typename F, typename UserTag>
MUDA_GLOBAL void muda::details::parallel_for_kernel (
    ParallelForCallable < F > f
) 
```




<hr>



### function stream\_error\_callback 

```C++
inline void muda::details::stream_error_callback (
    cudaStream_t stream,
    cudaError error,
    void * userdata
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/agent/kernel_assign.h`

