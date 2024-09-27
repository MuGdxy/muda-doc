

# Class muda::FieldEntryCore



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldEntryCore**](classmuda_1_1_field_entry_core.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**FieldEntryCore**](#function-fieldentrycore-13) () <br> |
|  MUDA\_GENERIC | [**FieldEntryCore**](#function-fieldentrycore-23) (std::byte \* buffer, const [**FieldEntryBaseData**](classmuda_1_1_field_entry_base_data.md) & info, [**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) name) <br> |
|  MUDA\_GENERIC | [**FieldEntryCore**](#function-fieldentrycore-33) (const [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) & rhs) = default<br> |
|  MUDA\_GENERIC std::byte \* | [**aos\_elem\_addr**](#function-aos_elem_addr-13) (int i) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aos\_elem\_addr**](#function-aos_elem_addr-23) (int i, int j) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aos\_elem\_addr**](#function-aos_elem_addr-33) (int i, int row\_index, int col\_index) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aos\_struct\_begin**](#function-aos_struct_begin) (int i) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aosoa\_elem\_addr**](#function-aosoa_elem_addr-13) (int i) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aosoa\_elem\_addr**](#function-aosoa_elem_addr-23) (int i, int j) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aosoa\_elem\_addr**](#function-aosoa_elem_addr-33) (int i, int row\_index, int col\_index) const<br> |
|  MUDA\_GENERIC uint32\_t | [**aosoa\_inner\_index**](#function-aosoa_inner_index) (int i) const<br> |
|  MUDA\_GENERIC std::byte \* | [**aosoa\_struct\_begin**](#function-aosoa_struct_begin) (int i) const<br> |
|  MUDA\_GENERIC T & | [**cast**](#function-cast-12) (std::byte \* data) <br> |
|  MUDA\_GENERIC const T & | [**cast**](#function-cast-22) (const std::byte \* data) const<br> |
|  MUDA\_GENERIC auto | [**count**](#function-count) () const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-13) (int i) const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-23) (int i, int j) const<br> |
|  MUDA\_GENERIC T \* | [**data**](#function-data-33) (int i, int row\_index, int col\_index) const<br> |
|  MUDA\_GENERIC std::byte \* | [**elem\_addr**](#function-elem_addr-13) (int i) const<br> |
|  MUDA\_GENERIC std::byte \* | [**elem\_addr**](#function-elem_addr-23) (int i, int j) const<br> |
|  MUDA\_GENERIC std::byte \* | [**elem\_addr**](#function-elem_addr-33) (int i, int row\_index, int col\_index) const<br> |
|  MUDA\_GENERIC auto | [**elem\_byte\_size**](#function-elem_byte_size) () const<br> |
|  MUDA\_GENERIC auto | [**layout**](#function-layout) () const<br> |
|  MUDA\_GENERIC auto | [**layout\_info**](#function-layout_info) () const<br> |
|  MUDA\_GENERIC auto | [**name**](#function-name) () const<br> |
|  MUDA\_GENERIC auto | [**name\_string\_pointer**](#function-name_string_pointer) () const<br> |
|  MUDA\_GENERIC auto | [**shape**](#function-shape) () const<br> |
|  MUDA\_GENERIC std::byte \* | [**soa\_elem\_addr**](#function-soa_elem_addr-13) (int i) const<br> |
|  MUDA\_GENERIC std::byte \* | [**soa\_elem\_addr**](#function-soa_elem_addr-23) (int i, int j) const<br> |
|  MUDA\_GENERIC std::byte \* | [**soa\_elem\_addr**](#function-soa_elem_addr-33) (int i, int row\_index, int col\_index) const<br> |
|  MUDA\_GENERIC auto | [**struct\_stride**](#function-struct_stride) () const<br> |




























## Public Functions Documentation




### function FieldEntryCore [1/3]

```C++
inline MUDA_GENERIC muda::FieldEntryCore::FieldEntryCore () 
```




<hr>



### function FieldEntryCore [2/3]

```C++
inline MUDA_GENERIC muda::FieldEntryCore::FieldEntryCore (
    std::byte * buffer,
    const FieldEntryBaseData & info,
    details::StringPointer name
) 
```




<hr>



### function FieldEntryCore [3/3]

```C++
MUDA_GENERIC muda::FieldEntryCore::FieldEntryCore (
    const FieldEntryCore & rhs
) = default
```




<hr>



### function aos\_elem\_addr [1/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aos_elem_addr (
    int i
) const
```




<hr>



### function aos\_elem\_addr [2/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aos_elem_addr (
    int i,
    int j
) const
```




<hr>



### function aos\_elem\_addr [3/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aos_elem_addr (
    int i,
    int row_index,
    int col_index
) const
```




<hr>



### function aos\_struct\_begin 

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aos_struct_begin (
    int i
) const
```




<hr>



### function aosoa\_elem\_addr [1/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aosoa_elem_addr (
    int i
) const
```




<hr>



### function aosoa\_elem\_addr [2/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aosoa_elem_addr (
    int i,
    int j
) const
```




<hr>



### function aosoa\_elem\_addr [3/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aosoa_elem_addr (
    int i,
    int row_index,
    int col_index
) const
```




<hr>



### function aosoa\_inner\_index 

```C++
MUDA_GENERIC uint32_t muda::FieldEntryCore::aosoa_inner_index (
    int i
) const
```




<hr>



### function aosoa\_struct\_begin 

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::aosoa_struct_begin (
    int i
) const
```




<hr>



### function cast [1/2]

```C++
template<typename T>
MUDA_GENERIC T & muda::FieldEntryCore::cast (
    std::byte * data
) 
```




<hr>



### function cast [2/2]

```C++
template<typename T>
MUDA_GENERIC const T & muda::FieldEntryCore::cast (
    const std::byte * data
) const
```




<hr>



### function count 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::count () const
```




<hr>



### function data [1/3]

```C++
template<typename T, FieldEntryLayout Layout>
inline MUDA_GENERIC T * muda::FieldEntryCore::data (
    int i
) const
```




<hr>



### function data [2/3]

```C++
template<typename T, FieldEntryLayout Layout>
inline MUDA_GENERIC T * muda::FieldEntryCore::data (
    int i,
    int j
) const
```




<hr>



### function data [3/3]

```C++
template<typename T, FieldEntryLayout Layout>
inline MUDA_GENERIC T * muda::FieldEntryCore::data (
    int i,
    int row_index,
    int col_index
) const
```




<hr>



### function elem\_addr [1/3]

```C++
template<FieldEntryLayout Layout>
MUDA_GENERIC std::byte * muda::FieldEntryCore::elem_addr (
    int i
) const
```




<hr>



### function elem\_addr [2/3]

```C++
template<FieldEntryLayout Layout>
MUDA_GENERIC std::byte * muda::FieldEntryCore::elem_addr (
    int i,
    int j
) const
```




<hr>



### function elem\_addr [3/3]

```C++
template<FieldEntryLayout Layout>
MUDA_GENERIC std::byte * muda::FieldEntryCore::elem_addr (
    int i,
    int row_index,
    int col_index
) const
```




<hr>



### function elem\_byte\_size 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::elem_byte_size () const
```




<hr>



### function layout 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::layout () const
```




<hr>



### function layout\_info 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::layout_info () const
```




<hr>



### function name 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::name () const
```




<hr>



### function name\_string\_pointer 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::name_string_pointer () const
```




<hr>



### function shape 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::shape () const
```




<hr>



### function soa\_elem\_addr [1/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::soa_elem_addr (
    int i
) const
```




<hr>



### function soa\_elem\_addr [2/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::soa_elem_addr (
    int i,
    int j
) const
```




<hr>



### function soa\_elem\_addr [3/3]

```C++
MUDA_GENERIC std::byte * muda::FieldEntryCore::soa_elem_addr (
    int i,
    int row_index,
    int col_index
) const
```




<hr>



### function struct\_stride 

```C++
inline MUDA_GENERIC auto muda::FieldEntryCore::struct_stride () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_entry_core.h`

