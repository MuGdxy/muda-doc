

# File compute\_graph\_fwd.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**compute\_graph\_fwd.h**](compute__graph__fwd_8h.md)

[Go to the documentation of this file](compute__graph__fwd_8h.md)


```C++
#pragma once
#include <muda/compute_graph/compute_graph_var_id.h>
#include <muda/compute_graph/compute_graph_closure_id.h>
#include <muda/compute_graph/compute_graph_node_id.h>
#include <muda/compute_graph/compute_graph_var_usage.h>
namespace muda
{
class ComputeGraphVarBase;
class ComputeGraphNodeBase;
class ComputeGraphVarManager;
class ComputeGraphClosure;
template <typename T>
class ComputeGraphVar;
class ComputeGraph;
class ComputeGraphGraphvizOptions;
namespace details
{
    class ComputeGraphAccessor;
}
}  // namespace muda
```


