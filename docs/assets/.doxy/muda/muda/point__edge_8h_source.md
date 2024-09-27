

# File point\_edge.h

[**File List**](files.md) **>** [**distance**](dir_eb002c7e2ab9cc8eedb85ee6f0f5ffd4.md) **>** [**point\_edge.h**](point__edge_8h.md)

[Go to the documentation of this file](point__edge_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>

namespace muda::distance
{
template <class T, int dim>
MUDA_GENERIC void point_edge_distance(const Eigen::Vector<T, dim>& p,
                                      const Eigen::Vector<T, dim>& e0,
                                      const Eigen::Vector<T, dim>& e1,
                                      T&                           dist2);

template <class T, int dim>
MUDA_GENERIC void point_edge_distance_gradient(const Eigen::Vector<T, dim>& p,
                                               const Eigen::Vector<T, dim>& e0,
                                               const Eigen::Vector<T, dim>& e1,
                                               Eigen::Vector<T, dim * 3>& grad);

template <class T, int dim>
MUDA_GENERIC void point_edge_distance_hessian(const Eigen::Vector<T, dim>& p,
                                              const Eigen::Vector<T, dim>& e0,
                                              const Eigen::Vector<T, dim>& e1,
                                              Eigen::Matrix<T, dim * 3, dim * 3>& Hessian);

}  // namespace muda::distance

#include "details/point_edge.inl"
```


