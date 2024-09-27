

# File edge\_edge.h

[**File List**](files.md) **>** [**distance**](dir_eb002c7e2ab9cc8eedb85ee6f0f5ffd4.md) **>** [**edge\_edge.h**](edge__edge_8h.md)

[Go to the documentation of this file](edge__edge_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>

namespace muda::distance
{
template <class T>
MUDA_GENERIC void edge_edge_distance(const Eigen::Vector<T, 3>& ea0,
                                     const Eigen::Vector<T, 3>& ea1,
                                     const Eigen::Vector<T, 3>& eb0,
                                     const Eigen::Vector<T, 3>& eb1,
                                     T&                         dist2);

template <class T>
MUDA_GENERIC void edge_edge_distance_gradient(const Eigen::Vector<T, 3>& ea0,
                                              const Eigen::Vector<T, 3>& ea1,
                                              const Eigen::Vector<T, 3>& eb0,
                                              const Eigen::Vector<T, 3>& eb1,
                                              Eigen::Vector<T, 12>&      grad);

template <class T>
MUDA_GENERIC void edge_edge_distance_hessian(const Eigen::Vector<T, 3>& ea0,
                                             const Eigen::Vector<T, 3>& ea1,
                                             const Eigen::Vector<T, 3>& eb0,
                                             const Eigen::Vector<T, 3>& eb1,
                                             Eigen::Matrix<T, 12, 12>& Hessian);

}  // namespace muda

#include "details/edge_edge.inl"
```


