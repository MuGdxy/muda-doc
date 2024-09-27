

# File compute\_graph\_dependency.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**compute\_graph\_dependency.h**](compute__graph__dependency_8h.md)

[Go to the documentation of this file](compute__graph__dependency_8h.md)


```C++
#pragma once
#include <muda/compute_graph/compute_graph_closure_id.h>
namespace muda
{
class ComputeGraphDependency
{
  public:
    ClosureId from;
    ClosureId to;
};
}  // namespace muda
```


