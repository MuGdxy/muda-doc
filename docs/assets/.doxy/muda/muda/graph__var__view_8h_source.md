

# File graph\_var\_view.h

[**File List**](files.md) **>** [**buffer**](dir_9b44f68c181db0b11e9502e462454d05.md) **>** [**graph\_var\_view.h**](graph__var__view_8h.md)

[Go to the documentation of this file](graph__var__view_8h.md)


```C++
#pragma once
#include <muda/buffer/var_view.h>
#include <muda/compute_graph/compute_graph_var.h>

namespace muda
{
template <typename T>
class ComputeGraphVar<VarView<T>> : public ComputeGraphVarBase
{
  public:
    static_assert(!std::is_const_v<T>, "T must not be const");

    using VarType = VarView<T>;
    using ROView  = CVarView<T>;
    using RWView  = VarView<T>;

  protected:
    friend class ComputeGraph;
    friend class ComputeGraphVarManager;

    using ComputeGraphVarBase::ComputeGraphVarBase;

    ComputeGraphVar(ComputeGraphVarManager* var_manager, std::string_view name, VarId var_id) MUDA_NOEXCEPT
        : ComputeGraphVarBase(var_manager, name, var_id)
    {
    }

    ComputeGraphVar(ComputeGraphVarManager* var_manager,
                    std::string_view        name,
                    VarId                   var_id,
                    const RWView&           init_value) MUDA_NOEXCEPT
        : ComputeGraphVarBase(var_manager, name, var_id, true),
          m_value(init_value)
    {
    }

    virtual ~ComputeGraphVar() = default;

  public:
    ROView ceval() const { return _ceval(m_value); }
    RWView eval() { return _eval(m_value); }
    auto   cviewer() const { return ceval().cviewer(); };
    auto   viewer() { return eval().viewer(); };
    operator ROView() const { return ceval(); }
    operator RWView() { return eval(); }

    void                      update(const RWView& view);
    ComputeGraphVar<VarType>& operator=(const RWView& view);

  private:
    RWView m_value;
};

}  // namespace muda

#include "details/graph_var_view.inl"
```


