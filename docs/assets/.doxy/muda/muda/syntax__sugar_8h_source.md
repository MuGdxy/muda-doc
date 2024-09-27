

# File syntax\_sugar.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**syntax\_sugar.h**](syntax__sugar_8h.md)

[Go to the documentation of this file](syntax__sugar_8h.md)


```C++
#pragma once

// usage:
// Launch().apply(
// [] $()
// {
//
// });
//
// you don't need to write mutable and __device__
#define $(...) MUDA_DEVICE(__VA_ARGS__) mutable

// usage:
// Launch().apply(
// [$def(viewer, buffer)] $()
// {
//
// });
#define $def(viewer, from) viewer = (from).name(#viewer)

// usage:
// ComputeGraph g;
// g.$node(name)
// {

// };
//
// you don't need to write g.create_node(name) << [&]
// {
//
// }
#define $node(name) create_node(name) << [&]

#define $kernel_name() kernel_name(__FUNCTION__)
```


