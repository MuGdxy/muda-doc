

# Namespace TCB\_SPAN\_NAMESPACE\_NAME::detail



[**Namespace List**](namespaces.md) **>** [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md) **>** [**detail**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail.md)




















## Classes

| Type | Name |
| ---: | :--- |
| struct | [**has\_size\_and\_data**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1has__size__and__data.md) &lt;typename, typename&gt;<br> |
| struct | [**has\_size\_and\_data**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1has__size__and__data.md) &lt;typename, typename&gt;<br> |
| struct | [**is\_complete**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__complete.md) &lt;typename, typename&gt;<br> |
| struct | [**is\_complete**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__complete.md) &lt;typename, typename&gt;<br> |
| struct | [**is\_container**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container.md) &lt;typename C, typename U&gt;<br> |
| struct | [**is\_container\_element\_type\_compatible**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container__element__type__compatible.md) &lt;typename, typename, typename&gt;<br> |
| struct | [**is\_container\_element\_type\_compatible**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container__element__type__compatible.md) &lt;typename, typename, typename&gt;<br> |
| struct | [**is\_span**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__span.md) &lt;typename&gt;<br> |
| struct | [**is\_span**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__span.md) &lt;typename&gt;<br> |
| struct | [**is\_std\_array**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__std__array.md) &lt;typename&gt;<br> |
| struct | [**is\_std\_array**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__std__array.md) &lt;typename&gt;<br> |
| struct | [**span\_storage**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1span__storage.md) &lt;typename E, S&gt;<br> |
| struct | [**span\_storage**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1span__storage.md) &lt;typename E, S&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef typename std::remove\_pointer&lt; T &gt;::type | [**remove\_pointer\_t**](#typedef-remove_pointer_t)  <br> |
| typedef typename std::remove\_cv&lt; typename std::remove\_reference&lt; T &gt;::type &gt;::type | [**uncvref\_t**](#typedef-uncvref_t)  <br> |
| typedef void | [**void\_t**](#typedef-void_t)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  decltype(c.data()) | [**data**](#function-data) (C & c) <br> |
|  decltype(c.data()) | [**data**](#function-data) (const C & c) <br> |
|  T \* | [**data**](#function-data) (T(&) array) noexcept<br> |
|  const E \* | [**data**](#function-data) (std::initializer\_list&lt; E &gt; il) noexcept<br> |
|  decltype(c.size()) | [**size**](#function-size) (const C & c) <br> |
|  std::size\_t | [**size**](#function-size) (const  T) noexcept<br> |




























## Public Types Documentation




### typedef remove\_pointer\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::detail::remove_pointer_t =  typename std::remove_pointer<T>::type;
```




<hr>



### typedef uncvref\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::detail::uncvref_t = 
    typename std::remove_cv<typename std::remove_reference<T>::type>::type;
```




<hr>



### typedef void\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::detail::void_t =  void;
```




<hr>
## Public Functions Documentation




### function data 

```C++
template<class C>
decltype(c.data()) TCB_SPAN_NAMESPACE_NAME::detail::data (
    C & c
) 
```




<hr>



### function data 

```C++
template<class C>
decltype(c.data()) TCB_SPAN_NAMESPACE_NAME::detail::data (
    const C & c
) 
```




<hr>



### function data 

```C++
template<class T, std::size_t N>
T * TCB_SPAN_NAMESPACE_NAME::detail::data (
    T(&) array
) noexcept
```




<hr>



### function data 

```C++
template<class E>
const E * TCB_SPAN_NAMESPACE_NAME::detail::data (
    std::initializer_list< E > il
) noexcept
```




<hr>



### function size 

```C++
template<class C>
decltype(c.size()) TCB_SPAN_NAMESPACE_NAME::detail::size (
    const C & c
) 
```




<hr>



### function size 

```C++
template<class T, std::size_t N>
std::size_t TCB_SPAN_NAMESPACE_NAME::detail::size (
    const T
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

