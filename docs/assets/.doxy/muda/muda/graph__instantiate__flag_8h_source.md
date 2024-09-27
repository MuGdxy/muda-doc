

# File graph\_instantiate\_flag.h

[**File List**](files.md) **>** [**graph**](dir_946c6946a1291bae853a7ff8b793a277.md) **>** [**graph\_instantiate\_flag.h**](graph__instantiate__flag_8h.md)

[Go to the documentation of this file](graph__instantiate__flag_8h.md)


```C++
#pragma once
#include <cuda.h>
#include <muda/tools/version.h>
namespace muda
{
enum class GraphInstantiateFlagBit
{
    FreeOnLaunch = CUgraphInstantiate_flags::CUDA_GRAPH_INSTANTIATE_FLAG_AUTO_FREE_ON_LAUNCH,
#if MUDA_WITH_DEVICE_STREAM_MODEL
    Upload = CUgraphInstantiate_flags::CUDA_GRAPH_INSTANTIATE_FLAG_UPLOAD,
    DeviceLaunch = CUgraphInstantiate_flags::CUDA_GRAPH_INSTANTIATE_FLAG_DEVICE_LAUNCH,
    UseNodePriority = CUgraphInstantiate_flags::CUDA_GRAPH_INSTANTIATE_FLAG_USE_NODE_PRIORITY,
#else
    Upload          = 2,
    DeviceLaunch    = 4,
    UseNodePriority = 8,
#endif
};
}  // namespace muda
```


