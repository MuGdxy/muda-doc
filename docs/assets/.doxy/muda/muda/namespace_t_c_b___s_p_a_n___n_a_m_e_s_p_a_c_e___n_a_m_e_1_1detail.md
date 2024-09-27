

# Namespace TCB\_SPAN\_NAMESPACE\_NAME::detail



[**Namespace List**](namespaces.md) **>** [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md) **>** [**detail**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail.md)




















## Classes

| Type | Name |
| ---: | :--- |
| struct | [**has\_size\_and\_data**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1has__size__and__data.md) &lt;typename, typename&gt;<br> |
| struct | [**has\_size\_and\_data&lt; T, void\_t&lt; decltype(detail::size(std::declval&lt; T &gt;())), decltype(detail::data(std::declval&lt; T &gt;()))&gt; &gt;**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1has__size__and__data_3_01_t_00fcf51269242c64e6f704600d32eb2114.md) &lt;typename T&gt;<br> |
| struct | [**is\_complete**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__complete.md) &lt;typename, typename&gt;<br> |
| struct | [**is\_complete&lt; T, decltype(sizeof(T))&gt;**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__complete_3_01_t_00_01decltype_07sizeof_07_t_08_08_4.md) &lt;typename T&gt;<br> |
| struct | [**is\_container**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container.md) &lt;typename C, typename U&gt;<br> |
| struct | [**is\_container\_element\_type\_compatible**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container__element__type__compatible.md) &lt;typename, typename, typename&gt;<br> |
| struct | [**is\_container\_element\_type\_compatible&lt; T, E, typename std::enable\_if&lt; !std::is\_same&lt; typename std::remove\_cv&lt; decltype(detail::data(std::declval&lt; T &gt;()))&gt;::type, void &gt;::value &&std::is\_convertible&lt; remove\_pointer\_t&lt; decltype(detail::data(std::declval&lt; T &gt;()))&gt;(\*)[], E(\*)[]&gt;::value &gt;::type &gt;**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__container__element__type__c072d1469943930dc7881b664700551d.md) &lt;typename T, typename E&gt;<br> |
| struct | [**is\_span**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__span.md) &lt;typename&gt;<br> |
| struct | [**is\_span&lt; span&lt; T, S &gt; &gt;**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__span_3_01span_3_01_t_00_01_s_01_4_01_4.md) &lt;typename T, S&gt;<br> |
| struct | [**is\_std\_array**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__std__array.md) &lt;typename&gt;<br> |
| struct | [**is\_std\_array&lt; std::array&lt; T, N &gt; &gt;**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1is__std__array_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4.md) &lt;typename T, N&gt;<br> |
| struct | [**span\_storage**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1span__storage.md) &lt;typename E, S&gt;<br> |
| struct | [**span\_storage&lt; E, dynamic\_extent &gt;**](struct_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail_1_1span__storage_3_01_e_00_01dynamic__extent_01_4.md) &lt;typename E&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef typename std::remove\_pointer&lt; T &gt;::type | [**remove\_pointer\_t**](#typedef-remove_pointer_t)  <br> |
| typedef typename std::remove\_cv&lt; typename std::remove\_reference&lt; T &gt;::type &gt;::type | [**uncvref\_t**](#typedef-uncvref_t)  <br> |
| typedef void | [**void\_t**](#typedef-void_t)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  constexpr auto | [**data**](#function-data) (C & c) <br> |
|  constexpr auto | [**data**](#function-data) (const C & c) <br> |
|  constexpr T \* | [**data**](#function-data) (T(&) array) noexcept<br> |
|  constexpr const E \* | [**data**](#function-data) (std::initializer\_list&lt; E &gt; il) noexcept<br> |
|  constexpr auto | [**size**](#function-size) (const C & c) <br> |
|  constexpr std::size\_t | [**size**](#function-size) (const  T) noexcept<br> |




























## Public Types Documentation




### typedef remove\_pointer\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::detail::remove_pointer_t = typedef typename std::remove_pointer<T>::type;
```




<hr>



### typedef uncvref\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::detail::uncvref_t = typedef typename std::remove_cv<typename std::remove_reference<T>::type>::type;
```




<hr>



### typedef void\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::detail::void_t = typedef void;
```




<hr>
## Public Functions Documentation




### function data 

```C++
template<class C>
constexpr auto TCB_SPAN_NAMESPACE_NAME::detail::data (
    C & c
) 
```




<hr>



### function data 

```C++
template<class C>
constexpr auto TCB_SPAN_NAMESPACE_NAME::detail::data (
    const C & c
) 
```




<hr>



### function data 

```C++
template<class T, std::size_t N>
constexpr T * TCB_SPAN_NAMESPACE_NAME::detail::data (
    T(&) array
) noexcept
```




<hr>



### function data 

```C++
template<class E>
constexpr const E * TCB_SPAN_NAMESPACE_NAME::detail::data (
    std::initializer_list< E > il
) noexcept
```




<hr>



### function size 

```C++
template<class C>
constexpr auto TCB_SPAN_NAMESPACE_NAME::detail::size (
    const C & c
) 
```




<hr>



### function size 

```C++
template<class T, std::size_t N>
constexpr std::size_t TCB_SPAN_NAMESPACE_NAME::detail::size (
    const T
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

