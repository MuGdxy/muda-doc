

# File compute\_graph\_phase.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**compute\_graph\_phase.h**](compute__graph__phase_8h.md)

[Go to the documentation of this file](compute__graph__phase_8h.md)


```C++
#pragma once
namespace muda
{
enum class ComputeGraphPhase
{
    None,
    TopoBuilding, // we don't create cuda graph at this point, just build the topo
    Building, // we create cuda graph at this point
    Updating, // we update the graph at this point
    SerialLaunching, // we just launch invoke all the graph closure in serial
    Max
};
}
```


