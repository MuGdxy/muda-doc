

# File string\_pointer.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**string\_pointer.h**](string__pointer_8h.md)

[Go to the documentation of this file](string__pointer_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>

namespace muda::details
{
class StringPointer
{
  public:
    char*        device_string = nullptr;
    char*        host_string   = nullptr;
    unsigned int length        = 0;

    MUDA_INLINE MUDA_GENERIC const char* auto_select() const MUDA_NOEXCEPT
    {
#ifdef __CUDA_ARCH__
        return device_string;
#else
        return host_string;
#endif  // __CUDA_ARCH__
    }
};
}  // namespace muda
```


