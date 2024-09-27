

# File linear\_system\_solve\_tolerance.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**linear\_system\_solve\_tolerance.h**](linear__system__solve__tolerance_8h.md)

[Go to the documentation of this file](linear__system__solve__tolerance_8h.md)


```C++
#pragma once
#include <numeric>

namespace muda
{
class LinearSystemSolveTolerance
{
    double m_solve_sparse_error_threshold = -1.0;

  public:
    void solve_sparse_error_threshold(double threshold)
    {
        m_solve_sparse_error_threshold = threshold;
    }

    template <typename T>
    T solve_sparse_error_threshold()
    {
        if(m_solve_sparse_error_threshold < 0.0)
        {
            constexpr auto eps = std::numeric_limits<T>::epsilon();
            return eps;
        }
        else
        {
            return static_cast<T>(m_solve_sparse_error_threshold);
        }
    }
};
}  // namespace muda
```


