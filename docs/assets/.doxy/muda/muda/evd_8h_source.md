

# File evd.h

[**File List**](files.md) **>** [**eigen**](dir_373cdbe7548ceaaa1c4b365fecb08d35.md) **>** [**evd.h**](evd_8h.md)

[Go to the documentation of this file](evd_8h.md)


```C++
#pragma once
#include <muda/muda_def.h>
#include <muda/ext/eigen/eigen_core_cxx20.h>
#include <Eigen/Eigenvalues>
namespace muda
{
namespace eigen
{
    template <typename T, int N>
    MUDA_GENERIC void evd(const Eigen::Matrix<T, N, N>& M,
                          Eigen::Vector<T, N>&          eigen_values,
                          Eigen::Matrix<T, N, N>&       eigen_vectors)
    {
        Eigen::SelfAdjointEigenSolver<Eigen::Matrix<T, N, N>> eigen_solver;
        // NOTE:
        //  On CUDA, if N <= 3, compute() is not supported.
        //  So, we use computeDirect() instead.
        if constexpr(N <= 3)
            eigen_solver.computeDirect(M);
        else
            eigen_solver.compute(M);
        eigen_values  = eigen_solver.eigenvalues();
        eigen_vectors = eigen_solver.eigenvectors();
    }
}  // namespace eigen
}  // namespace muda
```


