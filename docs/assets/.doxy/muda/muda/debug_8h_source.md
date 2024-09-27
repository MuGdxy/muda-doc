

# File debug.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**debug.h**](debug_8h.md)

[Go to the documentation of this file](debug_8h.md)


```C++
#pragma once
#include <atomic>
#include <muda/muda_config.h>
#include <mutex>
namespace muda
{
class Debug
{
  private:
    static auto& _is_debug_sync_all()
    {
        static std::atomic<bool> m_is_debug_sync_all(false);
        return m_is_debug_sync_all;
    }

    static auto& _mutex()
    {
        static std::mutex m_mutex;
        return m_mutex;
    }

    static auto& _sync_callback()
    {
        static std::function<void()> m_sync_callback = nullptr;
        return m_sync_callback;
    }

  public:
    static bool debug_sync_all(bool value)
    {
        _is_debug_sync_all() = value;
        return value;
    }

    static bool is_debug_sync_all() { return _is_debug_sync_all(); }

    static void set_sync_callback(std::function<void()> callback)
    {
        std::lock_guard<std::mutex> lock(_mutex());
        _sync_callback() = callback;
    }

    static void call_sync_callback()
    {
        if(_sync_callback())
        {
            _sync_callback()();
        }
    }
};
}  // namespace muda
```


