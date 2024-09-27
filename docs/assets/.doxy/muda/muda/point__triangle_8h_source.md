

# File point\_triangle.h

[**File List**](files.md) **>** [**distance**](dir_eb002c7e2ab9cc8eedb85ee6f0f5ffd4.md) **>** [**point\_triangle.h**](point__triangle_8h.md)

[Go to the documentation of this file](point__triangle_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>

namespace muda::distance
{
template <class T>
MUDA_GENERIC void point_triangle_distance(const Eigen::Vector<T, 3>& p,
                                          const Eigen::Vector<T, 3>& t0,
                                          const Eigen::Vector<T, 3>& t1,
                                          const Eigen::Vector<T, 3>& t2,
                                          T&                         dist2);

template <class T>
MUDA_GENERIC void point_triangle_distance_gradient(const Eigen::Vector<T, 3>& p,
                                                   const Eigen::Vector<T, 3>& t0,
                                                   const Eigen::Vector<T, 3>& t1,
                                                   const Eigen::Vector<T, 3>& t2,
                                                   Eigen::Vector<T, 12>& grad);

template <class T>
MUDA_GENERIC void point_triangle_distance_hessian(const Eigen::Vector<T, 3>& p,
                                                  const Eigen::Vector<T, 3>& t0,
                                                  const Eigen::Vector<T, 3>& t1,
                                                  const Eigen::Vector<T, 3>& t2,
                                                  Eigen::Matrix<T, 12, 12>& Hessian);
}  // namespace muda::distance

#include "details/point_triangle.inl"
```


