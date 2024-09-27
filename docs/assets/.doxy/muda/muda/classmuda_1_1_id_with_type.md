

# Class muda::IdWithType

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**IdWithType**](classmuda_1_1_id_with_type.md)










Inherited by the following classes: [muda::ClosureId](classmuda_1_1_closure_id.md),  [muda::NodeId](classmuda_1_1_node_id.md),  [muda::VarId](classmuda_1_1_var_id.md),  [muda::details::LocalVarId](classmuda_1_1details_1_1_local_var_id.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |






## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr auto | [**invalid\_id**](#variable-invalid_id)   = = std::numeric\_limits&lt;value\_type&gt;::max()<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**IdWithType**](#function-idwithtype-12) (value\_type value) noexcept<br> |
|  MUDA\_GENERIC | [**IdWithType**](#function-idwithtype-22) () noexcept<br> |
|  MUDA\_GENERIC bool | [**is\_valid**](#function-is_valid) () noexcept const<br> |
|  MUDA\_GENERIC value\_type | [**value**](#function-value) () noexcept const<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  value\_type | [**m\_value**](#variable-m_value)   = {invalid\_id}<br> |




















## Public Types Documentation




### typedef value\_type 

```C++
using muda::IdWithType< T >::value_type =  T;
```




<hr>
## Public Static Attributes Documentation




### variable invalid\_id 

```C++
constexpr auto muda::IdWithType< T >::invalid_id;
```




<hr>
## Public Functions Documentation




### function IdWithType [1/2]

```C++
inline explicit MUDA_GENERIC muda::IdWithType::IdWithType (
    value_type value
) noexcept
```




<hr>



### function IdWithType [2/2]

```C++
inline explicit MUDA_GENERIC muda::IdWithType::IdWithType () noexcept
```




<hr>



### function is\_valid 

```C++
inline MUDA_GENERIC bool muda::IdWithType::is_valid () noexcept const
```




<hr>



### function value 

```C++
inline MUDA_GENERIC value_type muda::IdWithType::value () noexcept const
```




<hr>
## Protected Attributes Documentation




### variable m\_value 

```C++
value_type muda::IdWithType< T >::m_value;
```




<hr>## Friends Documentation





### friend operator!= 

```C++
inline MUDA_GENERIC friend bool muda::IdWithType::operator!= (
    const IdWithType & lhs,
    const IdWithType & rhs
) noexcept
```




<hr>



### friend operator&lt; 

```C++
inline MUDA_GENERIC friend bool muda::IdWithType::operator< (
    const IdWithType & lhs,
    const IdWithType & rhs
) noexcept
```




<hr>



### friend operator&lt;&lt; 

```C++
inline std::ostream & muda::IdWithType::operator<< (
    std::ostream & os,
    const IdWithType & id
) 
```




<hr>



### friend operator== 

```C++
inline MUDA_GENERIC friend bool muda::IdWithType::operator== (
    const IdWithType & lhs,
    const IdWithType & rhs
) noexcept
```




<hr>



### friend operator&gt; 

```C++
inline MUDA_GENERIC friend bool muda::IdWithType::operator> (
    const IdWithType & lhs,
    const IdWithType & rhs
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/id_with_type.h`

