

# Class TCB\_SPAN\_NAMESPACE\_NAME::span

**template &lt;typename ElementType, std::size\_t Extent&gt;**



[**ClassList**](annotated.md) **>** [**TCB\_SPAN\_NAMESPACE\_NAME**](namespace_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e.md) **>** [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef const element\_type \* | [**const\_pointer**](#typedef-const_pointer)  <br> |
| typedef const element\_type & | [**const\_reference**](#typedef-const_reference)  <br> |
| typedef std::ptrdiff\_t | [**difference\_type**](#typedef-difference_type)  <br> |
| typedef ElementType | [**element\_type**](#typedef-element_type)  <br> |
| typedef pointer | [**iterator**](#typedef-iterator)  <br> |
| typedef element\_type \* | [**pointer**](#typedef-pointer)  <br> |
| typedef element\_type & | [**reference**](#typedef-reference)  <br> |
| typedef std::reverse\_iterator&lt; iterator &gt; | [**reverse\_iterator**](#typedef-reverse_iterator)  <br> |
| typedef std::size\_t | [**size\_type**](#typedef-size_type)  <br> |
| typedef [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; ElementType, Count !=dynamic\_extent ? Count :(Extent !=dynamic\_extent ? Extent - Offset :dynamic\_extent)&gt; | [**subspan\_return\_t**](#typedef-subspan_return_t)  <br> |
| typedef typename std::remove\_cv&lt; ElementType &gt;::type | [**value\_type**](#typedef-value_type)  <br> |






## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  size\_type | [**extent**](#variable-extent)   = = Extent<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|  TCB\_SPAN\_CONSTEXPR11 reference | [**back**](#function-back) () const<br> |
|  iterator | [**begin**](#function-begin) () noexcept const<br> |
|  pointer | [**data**](#function-data) () noexcept const<br> |
|  TCB\_SPAN\_NODISCARD constexpr bool | [**empty**](#function-empty) () noexcept const<br> |
|  iterator | [**end**](#function-end) () noexcept const<br> |
|  TCB\_SPAN\_CONSTEXPR11 [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; element\_type, Count &gt; | [**first**](#function-first-12) () const<br> |
|  TCB\_SPAN\_CONSTEXPR11 [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; element\_type, dynamic\_extent &gt; | [**first**](#function-first-22) (size\_type count) const<br> |
|  TCB\_SPAN\_CONSTEXPR11 reference | [**front**](#function-front) () const<br> |
|  TCB\_SPAN\_CONSTEXPR11 [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; element\_type, Count &gt; | [**last**](#function-last-12) () const<br> |
|  TCB\_SPAN\_CONSTEXPR11 [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; element\_type, dynamic\_extent &gt; | [**last**](#function-last-22) (size\_type count) const<br> |
|  TCB\_SPAN\_CONSTEXPR\_ASSIGN [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md) & | [**operator=**](#function-operator) (const [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md) & other) noexcept<br> |
|  TCB\_SPAN\_CONSTEXPR11 reference | [**operator[]**](#function-operator_1) (size\_type idx) const<br> |
|  TCB\_SPAN\_ARRAY\_CONSTEXPR reverse\_iterator | [**rbegin**](#function-rbegin) () noexcept const<br> |
|  TCB\_SPAN\_ARRAY\_CONSTEXPR reverse\_iterator | [**rend**](#function-rend) () noexcept const<br> |
|  size\_type | [**size**](#function-size) () noexcept const<br> |
|  size\_type | [**size\_bytes**](#function-size_bytes) () noexcept const<br> |
|  constexpr | [**span**](#function-span-110) () noexcept<br> |
|  TCB\_SPAN\_CONSTEXPR11 | [**span**](#function-span-210) (pointer ptr, size\_type count) <br> |
|  TCB\_SPAN\_CONSTEXPR11 | [**span**](#function-span-310) (pointer first\_elem, pointer last\_elem) <br> |
|  constexpr | [**span**](#function-span-410) (element\_type(&) arr) noexcept<br> |
|  TCB\_SPAN\_ARRAY\_CONSTEXPR | [**span**](#function-span-510) (std::array&lt; T, N &gt; & arr) noexcept<br> |
|  TCB\_SPAN\_ARRAY\_CONSTEXPR | [**span**](#function-span-610) (const std::array&lt; T, N &gt; & arr) noexcept<br> |
|  constexpr | [**span**](#function-span-710) (Container & cont) <br> |
|  constexpr | [**span**](#function-span-810) (const Container & cont) <br> |
|  constexpr | [**span**](#function-span-910) (const [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md) & other) noexcept<br> |
|  constexpr | [**span**](#function-span-1010) (const [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; OtherElementType, OtherExtent &gt; & other) noexcept<br> |
|  TCB\_SPAN\_CONSTEXPR11 [**subspan\_return\_t**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; Offset, Count &gt; | [**subspan**](#function-subspan-12) () const<br> |
|  TCB\_SPAN\_CONSTEXPR11 [**span**](class_t_c_b___s_p_a_n___n_a_m_e_s_p_a_c_e___n_a_m_e_1_1span.md)&lt; element\_type, dynamic\_extent &gt; | [**subspan**](#function-subspan-22) (size\_type offset, size\_type count=dynamic\_extent) const<br> |
|   | [**~span**](#function-span) () noexcept<br> |




























## Public Types Documentation




### typedef const\_pointer 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::const_pointer =  const element_type*;
```




<hr>



### typedef const\_reference 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::const_reference =  const element_type&;
```




<hr>



### typedef difference\_type 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::difference_type =  std::ptrdiff_t;
```




<hr>



### typedef element\_type 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::element_type =  ElementType;
```




<hr>



### typedef iterator 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::iterator =  pointer;
```




<hr>



### typedef pointer 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::pointer =  element_type*;
```




<hr>



### typedef reference 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::reference =  element_type&;
```




<hr>



### typedef reverse\_iterator 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::reverse_iterator =  std::reverse_iterator<iterator>;
```




<hr>



### typedef size\_type 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::size_type =  std::size_t;
```




<hr>



### typedef subspan\_return\_t 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::subspan_return_t = 
        span<ElementType, Count != dynamic_extent
                              ? Count
                              : (Extent != dynamic_extent ? Extent - Offset
                                                          : dynamic_extent)>;
```




<hr>



### typedef value\_type 

```C++
using TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::value_type =  typename std::remove_cv<ElementType>::type;
```




<hr>
## Public Static Attributes Documentation




### variable extent 

```C++
size_type TCB_SPAN_NAMESPACE_NAME::span< ElementType, Extent >::extent;
```




<hr>
## Public Functions Documentation




### function back 

```C++
inline TCB_SPAN_CONSTEXPR11 reference TCB_SPAN_NAMESPACE_NAME::span::back () const
```




<hr>



### function begin 

```C++
inline iterator TCB_SPAN_NAMESPACE_NAME::span::begin () noexcept const
```




<hr>



### function data 

```C++
inline pointer TCB_SPAN_NAMESPACE_NAME::span::data () noexcept const
```




<hr>



### function empty 

```C++
inline TCB_SPAN_NODISCARD constexpr bool TCB_SPAN_NAMESPACE_NAME::span::empty () noexcept const
```




<hr>



### function end 

```C++
inline iterator TCB_SPAN_NAMESPACE_NAME::span::end () noexcept const
```




<hr>



### function first [1/2]

```C++
template<std::size_t Count>
inline TCB_SPAN_CONSTEXPR11 span < element_type, Count > TCB_SPAN_NAMESPACE_NAME::span::first () const
```




<hr>



### function first [2/2]

```C++
inline TCB_SPAN_CONSTEXPR11 span < element_type, dynamic_extent > TCB_SPAN_NAMESPACE_NAME::span::first (
    size_type count
) const
```




<hr>



### function front 

```C++
inline TCB_SPAN_CONSTEXPR11 reference TCB_SPAN_NAMESPACE_NAME::span::front () const
```




<hr>



### function last [1/2]

```C++
template<std::size_t Count>
inline TCB_SPAN_CONSTEXPR11 span < element_type, Count > TCB_SPAN_NAMESPACE_NAME::span::last () const
```




<hr>



### function last [2/2]

```C++
inline TCB_SPAN_CONSTEXPR11 span < element_type, dynamic_extent > TCB_SPAN_NAMESPACE_NAME::span::last (
    size_type count
) const
```




<hr>



### function operator= 

```C++
TCB_SPAN_CONSTEXPR_ASSIGN span & TCB_SPAN_NAMESPACE_NAME::span::operator= (
    const span & other
) noexcept
```




<hr>



### function operator[] 

```C++
inline TCB_SPAN_CONSTEXPR11 reference TCB_SPAN_NAMESPACE_NAME::span::operator[] (
    size_type idx
) const
```




<hr>



### function rbegin 

```C++
inline TCB_SPAN_ARRAY_CONSTEXPR reverse_iterator TCB_SPAN_NAMESPACE_NAME::span::rbegin () noexcept const
```




<hr>



### function rend 

```C++
inline TCB_SPAN_ARRAY_CONSTEXPR reverse_iterator TCB_SPAN_NAMESPACE_NAME::span::rend () noexcept const
```




<hr>



### function size 

```C++
inline size_type TCB_SPAN_NAMESPACE_NAME::span::size () noexcept const
```




<hr>



### function size\_bytes 

```C++
inline size_type TCB_SPAN_NAMESPACE_NAME::span::size_bytes () noexcept const
```




<hr>



### function span [1/10]

```C++
template<std::size_t E, typename std::enable_if<(E==dynamic_extent||E<=0), int >::type>
inline constexpr TCB_SPAN_NAMESPACE_NAME::span::span () noexcept
```




<hr>



### function span [2/10]

```C++
inline TCB_SPAN_CONSTEXPR11 TCB_SPAN_NAMESPACE_NAME::span::span (
    pointer ptr,
    size_type count
) 
```




<hr>



### function span [3/10]

```C++
inline TCB_SPAN_CONSTEXPR11 TCB_SPAN_NAMESPACE_NAME::span::span (
    pointer first_elem,
    pointer last_elem
) 
```




<hr>



### function span [4/10]

```C++
template<std::size_t N, std::size_t E, typename std::enable_if<(E==dynamic_extent||N==E) && detail::is_container_element_type_compatible < element_type(&)[N], ElementType >::value, int >::type>
inline constexpr TCB_SPAN_NAMESPACE_NAME::span::span (
    element_type(&) arr
) noexcept
```




<hr>



### function span [5/10]

```C++
template<typename T, std::size_t N, std::size_t E, typename std::enable_if<(E==dynamic_extent||N==E) && detail::is_container_element_type_compatible < std::array< T, N > &, ElementType >::value, int >::type>
inline TCB_SPAN_ARRAY_CONSTEXPR TCB_SPAN_NAMESPACE_NAME::span::span (
    std::array< T, N > & arr
) noexcept
```




<hr>



### function span [6/10]

```C++
template<typename T, std::size_t N, std::size_t E, typename std::enable_if<(E==dynamic_extent||N==E) && detail::is_container_element_type_compatible < const std::array< T, N > &, ElementType >::value, int >::type>
inline TCB_SPAN_ARRAY_CONSTEXPR TCB_SPAN_NAMESPACE_NAME::span::span (
    const std::array< T, N > & arr
) noexcept
```




<hr>



### function span [7/10]

```C++
template<typename Container, std::size_t E, typename std::enable_if< E==dynamic_extent && detail::is_container < Container >::value && detail::is_container_element_type_compatible < Container &, ElementType >::value, int >::type>
inline constexpr TCB_SPAN_NAMESPACE_NAME::span::span (
    Container & cont
) 
```




<hr>



### function span [8/10]

```C++
template<typename Container, std::size_t E, typename std::enable_if< E==dynamic_extent && detail::is_container < Container >::value && detail::is_container_element_type_compatible < const Container &, ElementType >::value, int >::type>
inline constexpr TCB_SPAN_NAMESPACE_NAME::span::span (
    const Container & cont
) 
```




<hr>



### function span [9/10]

```C++
constexpr TCB_SPAN_NAMESPACE_NAME::span::span (
    const span & other
) noexcept
```




<hr>



### function span [10/10]

```C++
template<typename OtherElementType, std::size_t OtherExtent, typename std::enable_if<(Extent==dynamic_extent||OtherExtent==dynamic_extent||Extent==OtherExtent) &&std::is_convertible< OtherElementType(*)[], ElementType(*)[]>::value, int >::type>
inline constexpr TCB_SPAN_NAMESPACE_NAME::span::span (
    const span < OtherElementType, OtherExtent > & other
) noexcept
```




<hr>



### function subspan [1/2]

```C++
template<std::size_t Offset, std::size_t Count>
inline TCB_SPAN_CONSTEXPR11 subspan_return_t < Offset, Count > TCB_SPAN_NAMESPACE_NAME::span::subspan () const
```




<hr>



### function subspan [2/2]

```C++
inline TCB_SPAN_CONSTEXPR11 span < element_type, dynamic_extent > TCB_SPAN_NAMESPACE_NAME::span::subspan (
    size_type offset,
    size_type count=dynamic_extent
) const
```




<hr>



### function ~span 

```C++
TCB_SPAN_NAMESPACE_NAME::span::~span () noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/mstl/tcb/span.hpp`

