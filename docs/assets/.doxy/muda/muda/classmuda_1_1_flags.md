

# Class muda::Flags

**template &lt;typename BitType&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Flags**](classmuda_1_1_flags.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef BitType | [**bit\_type**](#typedef-bit_type)  <br> |
| typedef typename ::std::underlying\_type&lt; bit\_type &gt;::type | [**mask\_type**](#typedef-mask_type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC MUDA\_CONSTEXPR | [**Flags**](#function-flags-14) () <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR | [**Flags**](#function-flags-24) (BitType bit) <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR | [**Flags**](#function-flags-34) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR | [**Flags**](#function-flags-44) (mask\_type flags) <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**has**](#function-has) (BitType bit) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR | [**operator bool**](#function-operator-bool) () const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR | [**operator mask\_type**](#function-operator-mask_type) () const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator!**](#function-operator) () const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator!=**](#function-operator_1) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; | [**operator&**](#function-operator_2) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; & | [**operator&=**](#function-operator_3) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator&lt;**](#function-operator_4) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator&lt;=**](#function-operator_5) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; & | [**operator=**](#function-operator_6) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator==**](#function-operator_7) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator&gt;**](#function-operator_8) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR bool | [**operator&gt;=**](#function-operator_9) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; | [**operator^**](#function-operator_10) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; & | [**operator^=**](#function-operator_11) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) <br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; | [**operator\|**](#function-operator_12) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) const<br> |
|  MUDA\_GENERIC MUDA\_CONSTEXPR [**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; & | [**operator\|=**](#function-operator_13) ([**Flags**](classmuda_1_1_flags.md)&lt; BitType &gt; const & rhs) <br> |




























## Public Types Documentation




### typedef bit\_type 

```C++
using muda::Flags< BitType >::bit_type =  BitType;
```




<hr>



### typedef mask\_type 

```C++
using muda::Flags< BitType >::mask_type =  typename ::std::underlying_type<bit_type>::type;
```




<hr>
## Public Functions Documentation




### function Flags [1/4]

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR muda::Flags::Flags () 
```




<hr>



### function Flags [2/4]

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR muda::Flags::Flags (
    BitType bit
) 
```




<hr>



### function Flags [3/4]

```C++
MUDA_GENERIC MUDA_CONSTEXPR muda::Flags::Flags (
    Flags < BitType > const & rhs
) 
```




<hr>



### function Flags [4/4]

```C++
inline explicit MUDA_GENERIC MUDA_CONSTEXPR muda::Flags::Flags (
    mask_type flags
) 
```




<hr>



### function has 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::has (
    BitType bit
) const
```




<hr>



### function operator bool 

```C++
inline explicit MUDA_GENERIC MUDA_CONSTEXPR muda::Flags::operator bool () const
```




<hr>



### function operator mask\_type 

```C++
inline explicit MUDA_GENERIC MUDA_CONSTEXPR muda::Flags::operator mask_type () const
```




<hr>



### function operator! 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator! () const
```




<hr>



### function operator!= 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator!= (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator& 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > muda::Flags::operator& (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator&= 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > & muda::Flags::operator&= (
    Flags < BitType > const & rhs
) 
```




<hr>



### function operator&lt; 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator< (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator&lt;= 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator<= (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator= 

```C++
MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > & muda::Flags::operator= (
    Flags < BitType > const & rhs
) 
```




<hr>



### function operator== 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator== (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator&gt; 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator> (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator&gt;= 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR bool muda::Flags::operator>= (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator^ 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > muda::Flags::operator^ (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator^= 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > & muda::Flags::operator^= (
    Flags < BitType > const & rhs
) 
```




<hr>



### function operator\| 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > muda::Flags::operator| (
    Flags < BitType > const & rhs
) const
```




<hr>



### function operator\|= 

```C++
inline MUDA_GENERIC MUDA_CONSTEXPR Flags < BitType > & muda::Flags::operator|= (
    Flags < BitType > const & rhs
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/flag.h`

