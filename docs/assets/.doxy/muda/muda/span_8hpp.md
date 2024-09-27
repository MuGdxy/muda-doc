

# File span.hpp



[**FileList**](files.md) **>** [**mstl**](dir_76b30f276e6a3b8973955140272e7c63.md) **>** [**tcb**](dir_98b3ad4083edbdd3c811d05568c94a59.md) **>** [**span.hpp**](span_8hpp.md)

[Go to the source code of this file](span_8hpp_source.md)



* `#include <array>`
* `#include <cstddef>`
* `#include <cstdint>`
* `#include <type_traits>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md) <br> |
| namespace | [**detail**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail.md) <br> |
| namespace | [**std**](namespacestd.md) <br> |


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
| class | [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md) &lt;typename ElementType, Extent&gt;<br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**TCB\_SPAN\_ARRAY\_CONSTEXPR**](span_8hpp.md#define-tcb_span_array_constexpr)  <br> |
| define  | [**TCB\_SPAN\_CONSTEXPR11**](span_8hpp.md#define-tcb_span_constexpr11)  constexpr<br> |
| define  | [**TCB\_SPAN\_CONSTEXPR14**](span_8hpp.md#define-tcb_span_constexpr14)  <br> |
| define  | [**TCB\_SPAN\_CONSTEXPR\_ASSIGN**](span_8hpp.md#define-tcb_span_constexpr_assign)  <br> |
| define  | [**TCB\_SPAN\_EXPECT**](span_8hpp.md#define-tcb_span_expect) (cond) <br> |
| define  | [**TCB\_SPAN\_INLINE\_VAR**](span_8hpp.md#define-tcb_span_inline_var)  <br> |
| define  | [**TCB\_SPAN\_NAMESPACE\_NAME**](span_8hpp.md#define-tcb_span_namespace_name)  tcb<br> |
| define  | [**TCB\_SPAN\_NODISCARD**](span_8hpp.md#define-tcb_span_nodiscard)  <br> |
| define  | [**TCB\_SPAN\_NO\_CONTRACT\_CHECKING**](span_8hpp.md#define-tcb_span_no_contract_checking)  <br> |
| define  | [**TCB\_SPAN\_NO\_EXCEPTIONS**](span_8hpp.md#define-tcb_span_no_exceptions)  <br> |

## Macro Definition Documentation





### define TCB\_SPAN\_ARRAY\_CONSTEXPR 

```C++
#define TCB_SPAN_ARRAY_CONSTEXPR 
```




<hr>



### define TCB\_SPAN\_CONSTEXPR11 

```C++
#define TCB_SPAN_CONSTEXPR11 constexpr
```




<hr>



### define TCB\_SPAN\_CONSTEXPR14 

```C++
#define TCB_SPAN_CONSTEXPR14 
```




<hr>



### define TCB\_SPAN\_CONSTEXPR\_ASSIGN 

```C++
#define TCB_SPAN_CONSTEXPR_ASSIGN 
```




<hr>



### define TCB\_SPAN\_EXPECT 

```C++
#define TCB_SPAN_EXPECT (
    cond
) 
```




<hr>



### define TCB\_SPAN\_INLINE\_VAR 

```C++
#define TCB_SPAN_INLINE_VAR 
```




<hr>



### define TCB\_SPAN\_NAMESPACE\_NAME 

```C++
#define TCB_SPAN_NAMESPACE_NAME tcb
```




<hr>



### define TCB\_SPAN\_NODISCARD 

```C++
#define TCB_SPAN_NODISCARD 
```




<hr>



### define TCB\_SPAN\_NO\_CONTRACT\_CHECKING 

```C++
#define TCB_SPAN_NO_CONTRACT_CHECKING 
```




<hr>



### define TCB\_SPAN\_NO\_EXCEPTIONS 

```C++
#define TCB_SPAN_NO_EXCEPTIONS 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

