

# File cuda\_vec\_utils.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**cuda\_vec\_utils.h**](cuda__vec__utils_8h.md)

[Go to the documentation of this file](cuda__vec__utils_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <vector_types.h>

namespace muda
{
MUDA_INLINE MUDA_GENERIC int2 operator+(const int2& a, const int2& b)
{
    return make_int2(a.x + b.x, a.y + b.y);
}
}  // namespace muda
```


