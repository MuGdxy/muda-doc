

# Class muda::SubFieldInterface



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md)










Inherited by the following classes: [muda::SubFieldImpl](classmuda_1_1_sub_field_impl.md),  [muda::SubFieldImpl](classmuda_1_1_sub_field_impl.md),  [muda::SubFieldImpl](classmuda_1_1_sub_field_impl.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SubFieldInterface**](#function-subfieldinterface-13) ([**Field**](classmuda_1_1_field.md) & field) <br> |
|   | [**SubFieldInterface**](#function-subfieldinterface-23) (const [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &) = delete<br> |
|   | [**SubFieldInterface**](#function-subfieldinterface-33) ([**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &&) = delete<br> |
|  [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) & | [**operator=**](#function-operator) (const [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &) = delete<br> |
|  [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) & | [**operator=**](#function-operator_1) ([**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &&) = delete<br> |
| virtual  | [**~SubFieldInterface**](#function-subfieldinterface) () <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) | [**m\_build\_options**](#variable-m_build_options)  <br> |
|  std::byte \* | [**m\_data\_buffer**](#variable-m_data_buffer)   = = nullptr<br> |
|  size\_t | [**m\_data\_buffer\_size**](#variable-m_data_buffer_size)   = = 0<br> |
|  std::vector&lt; U&lt; [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) &gt; &gt; | [**m\_entries**](#variable-m_entries)  <br> |
|  [**Field**](classmuda_1_1_field.md) & | [**m\_field**](#variable-m_field)  <br> |
|  [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) | [**m\_layout\_info**](#variable-m_layout_info)  <br> |
|  std::unordered\_map&lt; std::string, size\_t &gt; | [**m\_name\_to\_index**](#variable-m_name_to_index)  <br> |
|  size\_t | [**m\_num\_elements**](#variable-m_num_elements)   = = 0<br> |
|  uint32\_t | [**m\_struct\_stride**](#variable-m_struct_stride)   = = ~0<br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual bool | [**allow\_inplace\_shrink**](#function-allow_inplace_shrink) () const<br> |
| virtual void | [**build\_impl**](#function-build_impl) () = 0<br> |
|  const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & | [**build\_options**](#function-build_options) () const<br> |
| virtual void | [**calculate\_new\_cores**](#function-calculate_new_cores) (std::byte \* byte\_buffer, size\_t total\_bytes, size\_t element\_count, span&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; new\_cores) = 0<br> |
|  const [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) & | [**layout\_info**](#function-layout_info) () const<br> |
|  size\_t | [**num\_elements**](#function-num_elements) () const<br> |
| virtual size\_t | [**require\_total\_buffer\_byte\_size**](#function-require_total_buffer_byte_size) (size\_t element\_count) = 0<br> |


## Protected Static Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**align**](#function-align) (uint32\_t offset, uint32\_t size, uint32\_t min\_alignment, uint32\_t max\_alignment) <br> |
|  uint32\_t | [**round\_up**](#function-round_up) (uint32\_t total, uint32\_t N) <br> |


## Public Functions Documentation




### function SubFieldInterface [1/3]

```C++
inline muda::SubFieldInterface::SubFieldInterface (
    Field & field
) 
```




<hr>



### function SubFieldInterface [2/3]

```C++
muda::SubFieldInterface::SubFieldInterface (
    const SubFieldInterface &
) = delete
```




<hr>



### function SubFieldInterface [3/3]

```C++
muda::SubFieldInterface::SubFieldInterface (
    SubFieldInterface &&
) = delete
```




<hr>



### function operator= 

```C++
SubFieldInterface & muda::SubFieldInterface::operator= (
    const SubFieldInterface &
) = delete
```




<hr>



### function operator= 

```C++
SubFieldInterface & muda::SubFieldInterface::operator= (
    SubFieldInterface &&
) = delete
```




<hr>



### function ~SubFieldInterface 

```C++
virtual muda::SubFieldInterface::~SubFieldInterface () 
```




<hr>
## Protected Attributes Documentation




### variable m\_build\_options 

```C++
FieldBuildOptions muda::SubFieldInterface::m_build_options;
```




<hr>



### variable m\_data\_buffer 

```C++
std::byte* muda::SubFieldInterface::m_data_buffer;
```




<hr>



### variable m\_data\_buffer\_size 

```C++
size_t muda::SubFieldInterface::m_data_buffer_size;
```




<hr>



### variable m\_entries 

```C++
std::vector<U<FieldEntryBase> > muda::SubFieldInterface::m_entries;
```




<hr>



### variable m\_field 

```C++
Field& muda::SubFieldInterface::m_field;
```




<hr>



### variable m\_layout\_info 

```C++
FieldEntryLayoutInfo muda::SubFieldInterface::m_layout_info;
```




<hr>



### variable m\_name\_to\_index 

```C++
std::unordered_map<std::string, size_t> muda::SubFieldInterface::m_name_to_index;
```




<hr>



### variable m\_num\_elements 

```C++
size_t muda::SubFieldInterface::m_num_elements;
```




<hr>



### variable m\_struct\_stride 

```C++
uint32_t muda::SubFieldInterface::m_struct_stride;
```




<hr>
## Protected Functions Documentation




### function allow\_inplace\_shrink 

```C++
inline virtual bool muda::SubFieldInterface::allow_inplace_shrink () const
```




<hr>



### function build\_impl 

```C++
virtual void muda::SubFieldInterface::build_impl () = 0
```




<hr>



### function build\_options 

```C++
inline const FieldBuildOptions & muda::SubFieldInterface::build_options () const
```




<hr>



### function calculate\_new\_cores 

```C++
virtual void muda::SubFieldInterface::calculate_new_cores (
    std::byte * byte_buffer,
    size_t total_bytes,
    size_t element_count,
    span< FieldEntryCore > new_cores
) = 0
```




<hr>



### function layout\_info 

```C++
inline const FieldEntryLayoutInfo & muda::SubFieldInterface::layout_info () const
```




<hr>



### function num\_elements 

```C++
inline size_t muda::SubFieldInterface::num_elements () const
```




<hr>



### function require\_total\_buffer\_byte\_size 

```C++
virtual size_t muda::SubFieldInterface::require_total_buffer_byte_size (
    size_t element_count
) = 0
```




<hr>
## Protected Static Functions Documentation




### function align 

```C++
static uint32_t muda::SubFieldInterface::align (
    uint32_t offset,
    uint32_t size,
    uint32_t min_alignment,
    uint32_t max_alignment
) 
```




<hr>



### function round\_up 

```C++
static uint32_t muda::SubFieldInterface::round_up (
    uint32_t total,
    uint32_t N
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/sub_field_interface.h`

