

# File cub\_wrapper.h

[**File List**](files.md) **>** [**cub**](dir_98c5d599fe44dff86fbf620b2a1f3e8e.md) **>** [**device**](dir_e7785ab0b6a4810de2e8c4f6e4ccf5c0.md) **>** [**cub\_wrapper.h**](cub__wrapper_8h.md)

[Go to the documentation of this file](cub__wrapper_8h.md)


```C++
#pragma once
#include <cub/version.cuh>
#include <muda/launch/launch_base.h>
#include <muda/buffer.h>
#include <muda/container.h>
#include <muda/buffer/buffer_launch.h>
#include <muda/compute_graph/compute_graph.h>
#include <muda/launch/stream.h>

namespace muda
{
template <typename Derive>
class CubWrapper : public LaunchBase<Derive>
{
  protected:
    std::byte* prepare_buffer(size_t reqSize)
    {
        return m_muda_stream->workspace(reqSize);
    }

  public:
    CubWrapper(Stream& stream = Stream::Default())
        : LaunchBase<Derive>(stream)
        , m_muda_stream(&stream)
    {
    }

    // meaningless for cub, so we just delete it
    void kernel_name(std::string_view) = delete;

    Stream* m_muda_stream = nullptr;
};
}  // namespace muda
```


