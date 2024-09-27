

# File svd.h

[**File List**](files.md) **>** [**eigen**](dir_373cdbe7548ceaaa1c4b365fecb08d35.md) **>** [**svd.h**](svd_8h.md)

[Go to the documentation of this file](svd_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>
#include <muda/ext/eigen/svd/svd_impl.h>

namespace muda
{
namespace eigen
{
    MUDA_GENERIC void svd(const Eigen::Matrix<float, 3, 3>& F,
                          Eigen::Matrix<float, 3, 3>&       U,
                          Eigen::Vector3<float>&            Sigma,
                          Eigen::Matrix<float, 3, 3>&       V);

    MUDA_GENERIC void pd(const Eigen::Matrix<float, 3, 3>& F,
                         Eigen::Matrix<float, 3, 3>&       R,
                         Eigen::Matrix<float, 3, 3>&       S);

    MUDA_GENERIC void svd(const Eigen::Matrix<double, 3, 3>& F,
                          Eigen::Matrix<double, 3, 3>&       U,
                          Eigen::Vector3<double>&            Sigma,
                          Eigen::Matrix<double, 3, 3>&       V);

    MUDA_GENERIC void pd(const Eigen::Matrix<double, 3, 3>& F,
                         Eigen::Matrix<double, 3, 3>&       R,
                         Eigen::Matrix<double, 3, 3>&       S);
}  // namespace eigen
}  // namespace muda
#include "details/svd.inl"
```


