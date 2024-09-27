

# File filesystem.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**filesystem.h**](filesystem_8h.md)

[Go to the documentation of this file](filesystem_8h.md)


```C++
#pragma once
#include <muda/tools/platform.h>

#ifdef MUDA_PLATFORM_LINUX
#if __GNUC__ >= 8
#include <filesystem>
namespace muda
{
    namespace filesystem = std::filesystem;
}
#else
#include <experimental/filesystem>
namespace muda
{
    namespace filesystem = std::experimental::filesystem;
}
#endif
#endif

#ifdef MUDA_PLATFORM_WINDOWS
#include <filesystem>
namespace muda
{
    namespace filesystem = std::filesystem;
}
#endif
```


