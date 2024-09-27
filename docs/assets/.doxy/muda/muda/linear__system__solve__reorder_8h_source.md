

# File linear\_system\_solve\_reorder.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**linear\_system\_solve\_reorder.h**](linear__system__solve__reorder_8h.md)

[Go to the documentation of this file](linear__system__solve__reorder_8h.md)


```C++
namespace muda
{
enum class LinearSystemReorderMethod
{
    None       = 0,
    Symrcm     = 1,
    Symamd     = 2,
    Csrmetisnd = 3,
};
class LinearSystemSolveReorder
{
    LinearSystemReorderMethod m_reorder_method = LinearSystemReorderMethod::None;

  public:
    LinearSystemReorderMethod reorder_method() const
    {
        return m_reorder_method;
    }
    void reoder_method(LinearSystemReorderMethod method)
    {
        m_reorder_method = method;
    }
    int reorder_method_int() const
    {
        return static_cast<int>(m_reorder_method);
    }
};
}  // namespace muda
```


