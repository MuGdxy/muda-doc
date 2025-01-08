

# Struct TCB\_SPAN\_NAMESPACE\_NAME::detail::span\_storage

**template &lt;typename E, std::size\_t S&gt;**



[**ClassList**](annotated.md) **>** [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md) **>** [**detail**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail.md) **>** [**span\_storage**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1span__storage.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  E \* | [**ptr**](#variable-ptr)   = = nullptr<br> |


## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  std::size\_t | [**size**](#variable-size)   = = S<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|  constexpr | [**span\_storage**](#function-span_storage-12) () noexcept<br> |
|  constexpr | [**span\_storage**](#function-span_storage-22) (E \* p\_ptr, std::size\_t) noexcept<br> |




























## Public Attributes Documentation




### variable ptr 

```C++
E* TCB_SPAN_NAMESPACE_NAME::detail::span_storage< E, S >::ptr;
```




<hr>
## Public Static Attributes Documentation




### variable size 

```C++
std::size_t TCB_SPAN_NAMESPACE_NAME::detail::span_storage< E, S >::size;
```




<hr>
## Public Functions Documentation




### function span\_storage [1/2]

```C++
constexpr TCB_SPAN_NAMESPACE_NAME::detail::span_storage::span_storage () noexcept
```




<hr>



### function span\_storage [2/2]

```C++
inline constexpr TCB_SPAN_NAMESPACE_NAME::detail::span_storage::span_storage (
    E * p_ptr,
    std::size_t
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

