

# Namespace TCB\_SPAN\_NAMESPACE\_NAME



[**Namespace List**](namespaces.md) **>** [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**detail**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1detail.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md) &lt;typename ElementType, Extent&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef unsigned char | [**byte**](#typedef-byte)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  TCB\_SPAN\_INLINE\_VAR constexpr std::size\_t | [**dynamic\_extent**](#variable-dynamic_extent)   = = SIZE\_MAX<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; const byte,((Extent==dynamic\_extent) ? dynamic\_extent :sizeof(ElementType) \*Extent)&gt; | [**as\_bytes**](#function-as_bytes) ([**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; ElementType, Extent &gt; s) noexcept<br> |
|  [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; byte,((Extent==dynamic\_extent) ? dynamic\_extent :sizeof(ElementType) \*Extent)&gt; | [**as\_writable\_bytes**](#function-as_writable_bytes) ([**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; ElementType, Extent &gt; s) noexcept<br> |
|  constexpr auto | [**get**](#function-get) ([**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; E, S &gt; s) <br> |
|  constexpr [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; ElementType, Extent &gt; | [**make\_span**](#function-make_span) ([**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; ElementType, Extent &gt; s) noexcept<br> |
|  constexpr [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; T, N &gt; | [**make\_span**](#function-make_span) (T(&) arr) noexcept<br> |
|  TCB\_SPAN\_ARRAY\_CONSTEXPR [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; T, N &gt; | [**make\_span**](#function-make_span) (std::array&lt; T, N &gt; & arr) noexcept<br> |
|  TCB\_SPAN\_ARRAY\_CONSTEXPR [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; const T, N &gt; | [**make\_span**](#function-make_span) (const std::array&lt; T, N &gt; & arr) noexcept<br> |
|  constexpr [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; typenamestd::remove\_reference&lt; decltype(\*detail::data(std::declval&lt; Container & &gt;()))&gt;::type | [**make\_span**](#function-make_span) (Container & cont) <br> |
|  constexpr [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; const typename Container::value\_type &gt; | [**make\_span**](#function-make_span) (const Container & cont) <br> |




























## Public Types Documentation




### typedef byte 

```C++
using TCB_SPAN_NAMESPACE_NAME::byte = typedef unsigned char;
```




<hr>
## Public Attributes Documentation




### variable dynamic\_extent 

```C++
TCB_SPAN_INLINE_VAR constexpr std::size_t TCB_SPAN_NAMESPACE_NAME::dynamic_extent;
```




<hr>
## Public Functions Documentation




### function as\_bytes 

```C++
template<typename ElementType, std::size_t Extent>
span < const byte,((Extent==dynamic_extent) ? dynamic_extent :sizeof(ElementType) *Extent)> TCB_SPAN_NAMESPACE_NAME::as_bytes (
    span < ElementType, Extent > s
) noexcept
```




<hr>



### function as\_writable\_bytes 

```C++
template<class ElementType, size_t Extent, typename std::enable_if<!std::is_const< ElementType >::value, int >::type>
span < byte,((Extent==dynamic_extent) ? dynamic_extent :sizeof(ElementType) *Extent)> TCB_SPAN_NAMESPACE_NAME::as_writable_bytes (
    span < ElementType, Extent > s
) noexcept
```




<hr>



### function get 

```C++
template<std::size_t N, typename E, std::size_t S>
constexpr auto TCB_SPAN_NAMESPACE_NAME::get (
    span < E, S > s
) 
```




<hr>



### function make\_span 

```C++
template<typename ElementType, std::size_t Extent>
constexpr span < ElementType, Extent > TCB_SPAN_NAMESPACE_NAME::make_span (
    span < ElementType, Extent > s
) noexcept
```




<hr>



### function make\_span 

```C++
template<typename T, std::size_t N>
constexpr span < T, N > TCB_SPAN_NAMESPACE_NAME::make_span (
    T(&) arr
) noexcept
```




<hr>



### function make\_span 

```C++
template<typename T, std::size_t N>
TCB_SPAN_ARRAY_CONSTEXPR span < T, N > TCB_SPAN_NAMESPACE_NAME::make_span (
    std::array< T, N > & arr
) noexcept
```




<hr>



### function make\_span 

```C++
template<typename T, std::size_t N>
TCB_SPAN_ARRAY_CONSTEXPR span < const T, N > TCB_SPAN_NAMESPACE_NAME::make_span (
    const std::array< T, N > & arr
) noexcept
```




<hr>



### function make\_span 

```C++
template<typename Container>
constexpr span < typenamestd::remove_reference< decltype(*detail::data(std::declval< Container & >()))>::type TCB_SPAN_NAMESPACE_NAME::make_span (
    Container & cont
) 
```




<hr>



### function make\_span 

```C++
template<typename Container>
constexpr span < const typename Container::value_type > TCB_SPAN_NAMESPACE_NAME::make_span (
    const Container & cont
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

