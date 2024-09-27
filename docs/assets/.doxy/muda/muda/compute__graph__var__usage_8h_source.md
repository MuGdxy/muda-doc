

# File compute\_graph\_var\_usage.h

[**File List**](files.md) **>** [**compute\_graph**](dir_b4aad8ec408afb185bc8426846668e86.md) **>** [**compute\_graph\_var\_usage.h**](compute__graph__var__usage_8h.md)

[Go to the documentation of this file](compute__graph__var__usage_8h.md)


```C++
#pragma once
namespace muda
{
enum class ComputeGraphVarUsage : char
{
    None,
    Read,
    ReadWrite,
    Max
};

inline bool operator<(ComputeGraphVarUsage lhs, ComputeGraphVarUsage rhs)
{
    return static_cast<char>(lhs) < static_cast<char>(rhs);
}

inline bool operator<=(ComputeGraphVarUsage lhs, ComputeGraphVarUsage rhs)
{
    return static_cast<char>(lhs) <= static_cast<char>(rhs);
}

inline bool operator>(ComputeGraphVarUsage lhs, ComputeGraphVarUsage rhs)
{
    return static_cast<char>(lhs) > static_cast<char>(rhs);
}

inline bool operator>=(ComputeGraphVarUsage lhs, ComputeGraphVarUsage rhs)
{
    return static_cast<char>(lhs) >= static_cast<char>(rhs);
}

inline bool operator==(ComputeGraphVarUsage lhs, ComputeGraphVarUsage rhs)
{
    return static_cast<char>(lhs) == static_cast<char>(rhs);
}
}  // namespace muda
```


