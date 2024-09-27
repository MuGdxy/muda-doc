

# File span.h

[**File List**](files.md) **>** [**mstl**](dir_76b30f276e6a3b8973955140272e7c63.md) **>** [**span.h**](span_8h.md)

[Go to the documentation of this file](span_8h.md)


```C++
#pragma once
#include <muda/tools/platform.h>
#include <muda/mstl/tcb/span.hpp>
#if MUDA_HAS_CXX20
#include <span>
#endif

namespace muda
{
#if MUDA_HAS_CXX20
using std::span;
#else
template <typename T>
using span = tcb::span<T>;
#endif
}  // namespace muda
```


