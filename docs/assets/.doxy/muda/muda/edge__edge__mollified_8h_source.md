

# File edge\_edge\_mollified.h

[**File List**](files.md) **>** [**distance**](dir_eb002c7e2ab9cc8eedb85ee6f0f5ffd4.md) **>** [**edge\_edge\_mollified.h**](edge__edge__mollified_8h.md)

[Go to the documentation of this file](edge__edge__mollified_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>

namespace muda::distance
{
template <class T>
MUDA_GENERIC void edge_edge_cross_norm2(const Eigen::Vector<T, 3>& ea0,
                                        const Eigen::Vector<T, 3>& ea1,
                                        const Eigen::Vector<T, 3>& eb0,
                                        const Eigen::Vector<T, 3>& eb1,
                                        T&                         result);

template <class T>
MUDA_GENERIC void edge_edge_cross_norm2_gradient(const Eigen::Vector<T, 3>& ea0,
                                                 const Eigen::Vector<T, 3>& ea1,
                                                 const Eigen::Vector<T, 3>& eb0,
                                                 const Eigen::Vector<T, 3>& eb1,
                                                 Eigen::Vector<T, 12>& grad);

template <class T>
MUDA_GENERIC void edge_edge_cross_norm2_hessian(const Eigen::Vector<T, 3>& ea0,
                                                const Eigen::Vector<T, 3>& ea1,
                                                const Eigen::Vector<T, 3>& eb0,
                                                const Eigen::Vector<T, 3>& eb1,
                                                Eigen::Matrix<T, 12, 12>& Hessian);

template <class T>
MUDA_GENERIC void edge_edge_mollifier(const Eigen::Vector<T, 3>& ea0,
                                      const Eigen::Vector<T, 3>& ea1,
                                      const Eigen::Vector<T, 3>& eb0,
                                      const Eigen::Vector<T, 3>& eb1,
                                      T                          eps_x,
                                      T&                         e);

template <class T>
MUDA_GENERIC void edge_edge_mollifier_gradient(const Eigen::Vector<T, 3>& ea0,
                                               const Eigen::Vector<T, 3>& ea1,
                                               const Eigen::Vector<T, 3>& eb0,
                                               const Eigen::Vector<T, 3>& eb1,
                                               T                          eps_x,
                                               Eigen::Vector<T, 12>&      g);

template <class T>
MUDA_GENERIC void edge_edge_mollifier_hessian(const Eigen::Vector<T, 3>& ea0,
                                              const Eigen::Vector<T, 3>& ea1,
                                              const Eigen::Vector<T, 3>& eb0,
                                              const Eigen::Vector<T, 3>& eb1,
                                              T                          eps_x,
                                              Eigen::Matrix<T, 12, 12>&  H);

template <class T>
MUDA_GENERIC void edge_edge_mollifier_threshold(const Eigen::Vector<T, 3>& ea0_rest,
                                                const Eigen::Vector<T, 3>& ea1_rest,
                                                const Eigen::Vector<T, 3>& eb0_rest,
                                                const Eigen::Vector<T, 3>& eb1_rest,
                                                T& eps_x);
}  // namespace muda::distance

#include "details/edge_edge_mollified.inl"
```


