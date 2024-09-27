

# Class muda::BufferLaunch



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**BufferLaunch**](classmuda_1_1_buffer_launch.md)








Inherits the following classes: [muda::LaunchBase](classmuda_1_1_launch_base.md)
















## Public Types inherited from muda::LaunchBase

See [muda::LaunchBase](classmuda_1_1_launch_base.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**derived\_type**](classmuda_1_1_launch_base.md#typedef-derived_type)  <br> |


























































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_HOST | [**BufferLaunch**](#function-bufferlaunch-13) (cudaStream\_t s=nullptr) <br> |
|  MUDA\_HOST | [**BufferLaunch**](#function-bufferlaunch-23) (int block\_dim, cudaStream\_t s=nullptr) <br> |
|  MUDA\_HOST | [**BufferLaunch**](#function-bufferlaunch-33) (int grid\_dim, int block\_dim, cudaStream\_t s=nullptr) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**alloc**](#function-alloc-13) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer, size\_t n) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**alloc**](#function-alloc-23) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer, [**Extent2D**](classmuda_1_1_extent2_d.md) extent) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**alloc**](#function-alloc-33) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer, [**Extent3D**](classmuda_1_1_extent3_d.md) extent) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**clear**](#function-clear-13) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**clear**](#function-clear-23) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**clear**](#function-clear-33) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-124) ([**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; dst, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-224) ([**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; dst, [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-324) ([**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; dst, [**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-424) ([**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; dst, [**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-524) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-624) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-724) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-824) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-924) (T \* dst, [**CVarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1024) (T \* dst, [**CBufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1124) (T \* dst, [**CBuffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1224) (T \* dst, [**CBuffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1324) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1424) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1524) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1624) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1724) ([**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; dst, const T \* src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1824) ([**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; dst, const T \* src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-1924) ([**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; dst, const T \* src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-2024) ([**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; dst, const T \* src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-2124) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-2224) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-2324) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**copy**](#function-copy-2424) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; &gt; & dst, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T \* &gt; & src) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-18) ([**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; buffer, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-28) ([**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; buffer, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-38) ([**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; buffer, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-48) ([**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; buffer, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-58) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**VarView**](classmuda_1_1_var_view_t.md)&lt; T &gt; &gt; & buffer, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-68) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**BufferView**](classmuda_1_1_buffer_view_t.md)&lt; T &gt; &gt; & buffer, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-78) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer2DView**](classmuda_1_1_buffer2_d_view_t.md)&lt; T &gt; &gt; & buffer, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**fill**](#function-fill-88) ([**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**Buffer3DView**](classmuda_1_1_buffer3_d_view_t.md)&lt; T &gt; &gt; & buffer, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**free**](#function-free-13) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**free**](#function-free-23) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**free**](#function-free-33) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**reserve**](#function-reserve-13) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer, size\_t capacity) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**reserve**](#function-reserve-23) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer, [**Extent2D**](classmuda_1_1_extent2_d.md) capacity) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**reserve**](#function-reserve-33) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer, [**Extent3D**](classmuda_1_1_extent3_d.md) capacity) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**resize**](#function-resize-19) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer, size\_t size) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**resize**](#function-resize-29) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer, [**Extent2D**](classmuda_1_1_extent2_d.md) extent) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**resize**](#function-resize-39) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer, [**Extent3D**](classmuda_1_1_extent3_d.md) extent) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**resize**](#function-resize-49) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer, size\_t size, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**resize**](#function-resize-59) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer, [**Extent2D**](classmuda_1_1_extent2_d.md) extent, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**resize**](#function-resize-69) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer, [**Extent3D**](classmuda_1_1_extent3_d.md) extent, const T & val) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**shrink\_to\_fit**](#function-shrink_to_fit-13) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**shrink\_to\_fit**](#function-shrink_to_fit-23) ([**DeviceBuffer2D**](classmuda_1_1_device_buffer2_d.md)&lt; T &gt; & buffer) <br> |
|  MUDA\_HOST [**BufferLaunch**](classmuda_1_1_buffer_launch.md) & | [**shrink\_to\_fit**](#function-shrink_to_fit-33) ([**DeviceBuffer3D**](classmuda_1_1_device_buffer3_d.md)&lt; T &gt; & buffer) <br> |


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




### function BufferLaunch [1/3]

```C++
inline MUDA_HOST muda::BufferLaunch::BufferLaunch (
    cudaStream_t s=nullptr
) 
```




<hr>



### function BufferLaunch [2/3]

```C++
inline MUDA_HOST muda::BufferLaunch::BufferLaunch (
    int block_dim,
    cudaStream_t s=nullptr
) 
```




<hr>



### function BufferLaunch [3/3]

```C++
inline MUDA_HOST muda::BufferLaunch::BufferLaunch (
    int grid_dim,
    int block_dim,
    cudaStream_t s=nullptr
) 
```




<hr>



### function alloc [1/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::alloc (
    DeviceBuffer < T > & buffer,
    size_t n
) 
```




<hr>



### function alloc [2/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::alloc (
    DeviceBuffer2D < T > & buffer,
    Extent2D extent
) 
```




<hr>



### function alloc [3/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::alloc (
    DeviceBuffer3D < T > & buffer,
    Extent3D extent
) 
```




<hr>



### function clear [1/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::clear (
    DeviceBuffer < T > & buffer
) 
```




<hr>



### function clear [2/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::clear (
    DeviceBuffer2D < T > & buffer
) 
```




<hr>



### function clear [3/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::clear (
    DeviceBuffer3D < T > & buffer
) 
```




<hr>



### function copy [1/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    VarView < T > dst,
    CVarView < T > src
) 
```




<hr>



### function copy [2/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    BufferView < T > dst,
    CBufferView < T > src
) 
```




<hr>



### function copy [3/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    Buffer2DView < T > dst,
    CBuffer2DView < T > src
) 
```




<hr>



### function copy [4/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    Buffer3DView < T > dst,
    CBuffer3DView < T > src
) 
```




<hr>



### function copy [5/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < VarView < T > > & dst,
    const ComputeGraphVar < VarView < T > > & src
) 
```




<hr>



### function copy [6/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < BufferView < T > > & dst,
    const ComputeGraphVar < BufferView < T > > & src
) 
```




<hr>



### function copy [7/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < Buffer2DView < T > > & dst,
    const ComputeGraphVar < Buffer2DView < T > > & src
) 
```




<hr>



### function copy [8/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < Buffer3DView < T > > & dst,
    const ComputeGraphVar < Buffer3DView < T > > & src
) 
```




<hr>



### function copy [9/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    T * dst,
    CVarView < T > src
) 
```




<hr>



### function copy [10/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    T * dst,
    CBufferView < T > src
) 
```




<hr>



### function copy [11/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    T * dst,
    CBuffer2DView < T > src
) 
```




<hr>



### function copy [12/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    T * dst,
    CBuffer3DView < T > src
) 
```




<hr>



### function copy [13/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < T * > & dst,
    const ComputeGraphVar < BufferView < T > > & src
) 
```




<hr>



### function copy [14/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < T * > & dst,
    const ComputeGraphVar < Buffer2DView < T > > & src
) 
```




<hr>



### function copy [15/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < T * > & dst,
    const ComputeGraphVar < VarView < T > > & src
) 
```




<hr>



### function copy [16/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < T * > & dst,
    const ComputeGraphVar < Buffer3DView < T > > & src
) 
```




<hr>



### function copy [17/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    VarView < T > dst,
    const T * src
) 
```




<hr>



### function copy [18/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    BufferView < T > dst,
    const T * src
) 
```




<hr>



### function copy [19/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    Buffer2DView < T > dst,
    const T * src
) 
```




<hr>



### function copy [20/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    Buffer3DView < T > dst,
    const T * src
) 
```




<hr>



### function copy [21/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < BufferView < T > > & dst,
    const ComputeGraphVar < T * > & src
) 
```




<hr>



### function copy [22/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < Buffer2DView < T > > & dst,
    const ComputeGraphVar < T * > & src
) 
```




<hr>



### function copy [23/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < VarView < T > > & dst,
    const ComputeGraphVar < T * > & src
) 
```




<hr>



### function copy [24/24]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::copy (
    ComputeGraphVar < Buffer3DView < T > > & dst,
    const ComputeGraphVar < T * > & src
) 
```




<hr>



### function fill [1/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    VarView < T > buffer,
    const T & val
) 
```




<hr>



### function fill [2/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    BufferView < T > buffer,
    const T & val
) 
```




<hr>



### function fill [3/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    Buffer2DView < T > buffer,
    const T & val
) 
```




<hr>



### function fill [4/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    Buffer3DView < T > buffer,
    const T & val
) 
```




<hr>



### function fill [5/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    ComputeGraphVar < VarView < T > > & buffer,
    const ComputeGraphVar < T > & val
) 
```




<hr>



### function fill [6/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    ComputeGraphVar < BufferView < T > > & buffer,
    const ComputeGraphVar < T > & val
) 
```




<hr>



### function fill [7/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    ComputeGraphVar < Buffer2DView < T > > & buffer,
    const ComputeGraphVar < T > & val
) 
```




<hr>



### function fill [8/8]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::fill (
    ComputeGraphVar < Buffer3DView < T > > & buffer,
    const ComputeGraphVar < T > & val
) 
```




<hr>



### function free [1/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::free (
    DeviceBuffer < T > & buffer
) 
```




<hr>



### function free [2/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::free (
    DeviceBuffer2D < T > & buffer
) 
```




<hr>



### function free [3/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::free (
    DeviceBuffer3D < T > & buffer
) 
```




<hr>



### function reserve [1/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::reserve (
    DeviceBuffer < T > & buffer,
    size_t capacity
) 
```




<hr>



### function reserve [2/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::reserve (
    DeviceBuffer2D < T > & buffer,
    Extent2D capacity
) 
```




<hr>



### function reserve [3/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::reserve (
    DeviceBuffer3D < T > & buffer,
    Extent3D capacity
) 
```




<hr>



### function resize [1/9]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::resize (
    DeviceBuffer < T > & buffer,
    size_t size
) 
```




<hr>



### function resize [2/9]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::resize (
    DeviceBuffer2D < T > & buffer,
    Extent2D extent
) 
```




<hr>



### function resize [3/9]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::resize (
    DeviceBuffer3D < T > & buffer,
    Extent3D extent
) 
```




<hr>



### function resize [4/9]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::resize (
    DeviceBuffer < T > & buffer,
    size_t size,
    const T & val
) 
```




<hr>



### function resize [5/9]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::resize (
    DeviceBuffer2D < T > & buffer,
    Extent2D extent,
    const T & val
) 
```




<hr>



### function resize [6/9]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::resize (
    DeviceBuffer3D < T > & buffer,
    Extent3D extent,
    const T & val
) 
```




<hr>



### function shrink\_to\_fit [1/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::shrink_to_fit (
    DeviceBuffer < T > & buffer
) 
```




<hr>



### function shrink\_to\_fit [2/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::shrink_to_fit (
    DeviceBuffer2D < T > & buffer
) 
```




<hr>



### function shrink\_to\_fit [3/3]

```C++
template<typename T>
MUDA_HOST BufferLaunch & muda::BufferLaunch::shrink_to_fit (
    DeviceBuffer3D < T > & buffer
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/buffer_launch.h`

