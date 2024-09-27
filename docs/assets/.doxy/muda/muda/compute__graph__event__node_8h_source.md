

# File compute\_graph\_event\_node.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**nodes**](dir_7ff8159720d09b9da5f49b4c95af33a4.md) **>** [**compute\_graph\_event\_node.h**](compute__graph__event__node_8h.md)

[Go to the documentation of this file](compute__graph__event__node_8h.md)


```C++
#pragma once
#include <muda/compute_graph/compute_graph.h>
#include <muda/compute_graph/compute_graph_node.h>
#include <muda/graph/graph.h>
#include <muda/graph/event_node.h>

namespace muda
{
using ComputeGraphEventRecordNode =
    ComputeGraphNode<EventRecordNode, ComputeGraphNodeType::EventRecordNode>;
using ComputeGraphEventWaitNode =
    ComputeGraphNode<EventWaitNode, ComputeGraphNodeType::EventWaitNode>;
}  // namespace muda
```


