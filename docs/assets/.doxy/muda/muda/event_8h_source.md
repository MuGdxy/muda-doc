

# File event.h

[**File List**](files.md) **>** [**launch**](dir_440d6ef7395341c98b5d944289d06a83.md) **>** [**event.h**](event_8h.md)

[Go to the documentation of this file](event_8h.md)


```C++
#pragma once
#include <muda/tools/flag.h>
#include <cuda.h>
#include <cuda_runtime.h>
#include <cuda_runtime_api.h>
#include <device_launch_parameters.h>
#include <muda/check/check_cuda_errors.h>

namespace muda
{
class Event
{
    cudaEvent_t m_handle = nullptr;

  public:
    enum class Bit : unsigned int
    {
        eDefault = cudaEventDefault,           
        eBlockingSync = cudaEventBlockingSync, 
        eDisableTiming = cudaEventDisableTiming, 
        eInterprocess = cudaEventInterprocess 
    };

    enum class QueryResult
    {
        eFinished = cudaSuccess,       
        eNotReady = cudaErrorNotReady, 
    };

    Event(Flags<Bit> flag = Bit::eDisableTiming);
    ~Event();

    QueryResult query() const;
    // elapsed time (in ms) between two events
    static float elapsed_time(cudaEvent_t start, cudaEvent_t stop);

    operator cudaEvent_t() { return m_handle; }
    cudaEvent_t viewer() const { return m_handle; }

    // delete copy constructor and assignment operator
    Event(const Event&)            = delete;
    Event& operator=(const Event&) = delete;

    // allow move constructor
    Event(Event&& o) MUDA_NOEXCEPT;
    // delete move assignment operator
    Event& operator=(Event&& o) MUDA_NOEXCEPT;
};
}  // namespace muda

#include "details/event.inl"
```


