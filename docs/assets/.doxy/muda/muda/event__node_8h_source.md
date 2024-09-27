

# File event\_node.h

[**File List**](files.md) **>** [**graph**](dir_946c6946a1291bae853a7ff8b793a277.md) **>** [**event\_node.h**](event__node_8h.md)

[Go to the documentation of this file](event__node_8h.md)


```C++
#pragma once
#include <muda/graph/graph_base.h>

namespace muda
{
class EventRecordNode : public GraphNode
{
  public:
    using this_type = EventRecordNode;
    friend class Graph;
};

class EventWaitNode : public GraphNode
{
  public:
    using this_type = EventWaitNode;
    friend class Graph;
};
}  // namespace muda
```


