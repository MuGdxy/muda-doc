

# File sparse\_spatial\_hash.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**geo**](dir_e05e4ae50bce28830f3a7b1d7f2eeff2.md) **>** [**spatial\_hash**](dir_58b30d2a266b6e98a9cbea81c385691b.md) **>** [**sparse\_spatial\_hash.h**](sparse__spatial__hash_8h.md)

[Go to the documentation of this file](sparse__spatial__hash_8h.md)


```C++
#pragma once
#include <muda/ext/geo/spatial_hash/sparse_spatial_hash_impl.h>

namespace muda::spatial_hash
{
class DefaultPredication
{
  public:
    __device__ bool operator()(int i, int j) { return true; }
};

template <typename Hash = Morton<uint32_t>>
class SparseSpatialHash
{
    // algorithm comes from:
    // https://developer.nvidia.com/gpugems/gpugems3/part-v-physics-simulation/chapter-32-broad-phase-collision-detection-cuda
  private:
    using Impl = details::SparseSpatialHashImpl<Hash>;

    Impl m_impl;

  public:
    SparseSpatialHash(muda::Stream& stream = muda::Stream::Default())
        : m_impl(stream)
    {
    }

    template <typename Pred = DefaultPredication>
    void detect(CBufferView<BoundingSphere>  spheres,
                DeviceBuffer<CollisionPair>& collisionPairs,
                Pred&&                       pred = {})
    {
        m_impl.level = 0;
        m_impl.detect(spheres, false, collisionPairs, std::forward<Pred>(pred));
    }

    template <typename Pred = DefaultPredication>
    void detect(int                          level,
                CBufferView<BoundingSphere>  spheres,
                DeviceBuffer<CollisionPair>& collisionPairs,
                Pred&&                       pred = {})
    {
        MUDA_KERNEL_ASSERT(level >= 0, "invalid level");
        m_impl.level = level;
        m_impl.detect(spheres, true, collisionPairs, std::forward<Pred>(pred));
    }
};
}  // namespace muda::spatial_hash
```


