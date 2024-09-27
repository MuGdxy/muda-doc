

# Struct TCB\_SPAN\_NAMESPACE\_NAME::detail::is\_container

**template &lt;typename C, typename U&gt;**



[**ClassList**](annotated.md) **>** [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md) **>** [**detail**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail.md) **>** [**is\_container**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container.md)




























## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**value**](#variable-value)   = =
        ![**is\_span**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__span.md)&lt;U&gt;::value && ![**is\_std\_array**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__std__array.md)&lt;U&gt;::value &&
        !std::is\_array&lt;U&gt;::value && [**has\_size\_and\_data**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1has__size__and__data.md)&lt;C&gt;::value<br> |










































## Public Static Attributes Documentation




### variable value 

```C++
constexpr bool TCB_SPAN_NAMESPACE_NAME::detail::is_container< C, U >::value;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

