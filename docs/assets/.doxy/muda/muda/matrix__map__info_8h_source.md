

# File matrix\_map\_info.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**field**](dir_67616bafb1e973d10aec465c6be4ad46.md) **>** [**matrix\_map\_info.h**](matrix__map__info_8h.md)

[Go to the documentation of this file](matrix__map__info_8h.md)


```C++
#pragma once

namespace muda
{
template <typename T, int M, int N>
class MatrixMapInfo
{
  public:
    T*  begin;
    int outer_stride;
    int inner_stride;
};

template <typename T, int M, int N>
class CMatrixMapInfo
{
  public:
    const T*  begin;
    int outer_stride;
    int inner_stride;
};
}  // namespace muda
```


