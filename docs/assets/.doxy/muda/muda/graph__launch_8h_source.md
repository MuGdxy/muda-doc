

# File graph\_launch.h

[**File List**](files.md) **>** [**graph**](dir_946c6946a1291bae853a7ff8b793a277.md) **>** [**graph\_launch.h**](graph__launch_8h.md)

[Go to the documentation of this file](graph__launch_8h.md)


```C++
#pragma once
#include <muda/launch/launch_base.h>

namespace muda
{
class GraphViewer;
class GraphLaunch : public LaunchBase<GraphLaunch>
{
  public:
    GraphLaunch(cudaStream_t stream = nullptr)
        : LaunchBase(stream)
    {
    }
    ~GraphLaunch() = default;

    GraphLaunch& launch(const GraphViewer& graph);
};
}  // namespace muda

#include "details/graph_launch.inl"
```


