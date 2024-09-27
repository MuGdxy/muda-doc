

# File point\_point.h

[**File List**](files.md) **>** [**distance**](dir_eb002c7e2ab9cc8eedb85ee6f0f5ffd4.md) **>** [**point\_point.h**](point__point_8h.md)

[Go to the documentation of this file](point__point_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>

namespace muda::distance
{
template <class T, int dim>
MUDA_GENERIC void point_point_distance(const Eigen::Vector<T, dim>& a,
                                       const Eigen::Vector<T, dim>& b,
                                       T&                           dist2);

template <class T, int dim>
MUDA_GENERIC void point_point_distance_gradient(const Eigen::Vector<T, dim>& a,
                                                const Eigen::Vector<T, dim>& b,
                                                Eigen::Vector<T, dim * 2>& grad);

template <class T, int dim>
MUDA_GENERIC void point_point_distance_hessian(const Eigen::Vector<T, dim>& a,
                                               const Eigen::Vector<T, dim>& b,
                                               Eigen::Matrix<T, dim * 2, dim * 2>& Hessian);
}  // namespace muda::distance

#include "details/point_point.inl"
```


