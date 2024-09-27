

# File compute\_graph\_flag.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**compute\_graph\_flag.h**](compute__graph__flag_8h.md)

[Go to the documentation of this file](compute__graph__flag_8h.md)


```C++
#pragma once
namespace muda
{
enum class ComputeGraphFlag
{
    HostLaunch   = 1,
    DeviceLaunch = 2 | HostLaunch,
};
}
```


