

# Class muda::SubFieldImpl&lt; FieldEntryLayout::SoA &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**SubFieldImpl&lt; FieldEntryLayout::SoA &gt;**](classmuda_1_1_sub_field_impl_3_01_field_entry_layout_1_1_so_a_01_4.md)








Inherits the following classes: [muda::SubFieldInterface](classmuda_1_1_sub_field_interface.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SubFieldInterface**](#function-subfieldinterface-13) ([**Field**](classmuda_1_1_field.md) & field) <br> |
|   | [**SubFieldInterface**](#function-subfieldinterface-23) (const [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &) = delete<br> |
|   | [**SubFieldInterface**](#function-subfieldinterface-33) ([**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &&) = delete<br> |
| virtual  | [**~SubFieldImpl**](#function-subfieldimpl) () override<br> |


## Public Functions inherited from muda::SubFieldInterface

See [muda::SubFieldInterface](classmuda_1_1_sub_field_interface.md)

| Type | Name |
| ---: | :--- |
|   | [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md#function-subfieldinterface-13) ([**Field**](classmuda_1_1_field.md) & field) <br> |
|   | [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md#function-subfieldinterface-23) (const [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &) = delete<br> |
|   | [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md#function-subfieldinterface-33) ([**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &&) = delete<br> |
|  [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) & | [**operator=**](classmuda_1_1_sub_field_interface.md#function-operator) (const [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &) = delete<br> |
|  [**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) & | [**operator=**](classmuda_1_1_sub_field_interface.md#function-operator_1) ([**SubFieldInterface**](classmuda_1_1_sub_field_interface.md) &&) = delete<br> |
| virtual  | [**~SubFieldInterface**](classmuda_1_1_sub_field_interface.md#function-subfieldinterface) () <br> |
















## Protected Attributes inherited from muda::SubFieldInterface

See [muda::SubFieldInterface](classmuda_1_1_sub_field_interface.md)

| Type | Name |
| ---: | :--- |
|  [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) | [**m\_build\_options**](classmuda_1_1_sub_field_interface.md#variable-m_build_options)  <br> |
|  std::byte \* | [**m\_data\_buffer**](classmuda_1_1_sub_field_interface.md#variable-m_data_buffer)   = = nullptr<br> |
|  size\_t | [**m\_data\_buffer\_size**](classmuda_1_1_sub_field_interface.md#variable-m_data_buffer_size)   = = 0<br> |
|  std::vector&lt; U&lt; [**FieldEntryBase**](classmuda_1_1_field_entry_base.md) &gt; &gt; | [**m\_entries**](classmuda_1_1_sub_field_interface.md#variable-m_entries)  <br> |
|  [**Field**](classmuda_1_1_field.md) & | [**m\_field**](classmuda_1_1_sub_field_interface.md#variable-m_field)  <br> |
|  [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) | [**m\_layout\_info**](classmuda_1_1_sub_field_interface.md#variable-m_layout_info)  <br> |
|  std::unordered\_map&lt; std::string, size\_t &gt; | [**m\_name\_to\_index**](classmuda_1_1_sub_field_interface.md#variable-m_name_to_index)  <br> |
|  size\_t | [**m\_num\_elements**](classmuda_1_1_sub_field_interface.md#variable-m_num_elements)   = = 0<br> |
|  uint32\_t | [**m\_struct\_stride**](classmuda_1_1_sub_field_interface.md#variable-m_struct_stride)   = = ~0<br> |






























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual bool | [**allow\_inplace\_shrink**](#function-allow_inplace_shrink) () const<br> |
| virtual void | [**build\_impl**](#function-build_impl) () override<br> |
| virtual void | [**calculate\_new\_cores**](#function-calculate_new_cores) (std::byte \* byte\_buffer, size\_t total\_bytes, size\_t element\_count, span&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; new\_cores) override<br> |
| virtual size\_t | [**require\_total\_buffer\_byte\_size**](#function-require_total_buffer_byte_size) (size\_t element\_count) override<br> |


## Protected Functions inherited from muda::SubFieldInterface

See [muda::SubFieldInterface](classmuda_1_1_sub_field_interface.md)

| Type | Name |
| ---: | :--- |
| virtual bool | [**allow\_inplace\_shrink**](classmuda_1_1_sub_field_interface.md#function-allow_inplace_shrink) () const<br> |
| virtual void | [**build\_impl**](classmuda_1_1_sub_field_interface.md#function-build_impl) () = 0<br> |
|  const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & | [**build\_options**](classmuda_1_1_sub_field_interface.md#function-build_options) () const<br> |
| virtual void | [**calculate\_new\_cores**](classmuda_1_1_sub_field_interface.md#function-calculate_new_cores) (std::byte \* byte\_buffer, size\_t total\_bytes, size\_t element\_count, span&lt; [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) &gt; new\_cores) = 0<br> |
|  const [**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) & | [**layout\_info**](classmuda_1_1_sub_field_interface.md#function-layout_info) () const<br> |
|  size\_t | [**num\_elements**](classmuda_1_1_sub_field_interface.md#function-num_elements) () const<br> |
| virtual size\_t | [**require\_total\_buffer\_byte\_size**](classmuda_1_1_sub_field_interface.md#function-require_total_buffer_byte_size) (size\_t element\_count) = 0<br> |




## Protected Static Functions inherited from muda::SubFieldInterface

See [muda::SubFieldInterface](classmuda_1_1_sub_field_interface.md)

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**align**](classmuda_1_1_sub_field_interface.md#function-align) (uint32\_t offset, uint32\_t size, uint32\_t min\_alignment, uint32\_t max\_alignment) <br> |
|  uint32\_t | [**round\_up**](classmuda_1_1_sub_field_interface.md#function-round_up) (uint32\_t total, uint32\_t N) <br> |


## Public Functions Documentation




### function SubFieldInterface [1/3]

```C++
inline muda::SubFieldImpl< FieldEntryLayout::SoA >::SubFieldInterface (
    Field & field
) 
```




<hr>



### function SubFieldInterface [2/3]

```C++
muda::SubFieldImpl< FieldEntryLayout::SoA >::SubFieldInterface (
    const SubFieldInterface &
) = delete
```




<hr>



### function SubFieldInterface [3/3]

```C++
muda::SubFieldImpl< FieldEntryLayout::SoA >::SubFieldInterface (
    SubFieldInterface &&
) = delete
```




<hr>



### function ~SubFieldImpl 

```C++
virtual muda::SubFieldImpl< FieldEntryLayout::SoA >::~SubFieldImpl () override
```




<hr>
## Protected Functions Documentation




### function allow\_inplace\_shrink 

```C++
inline virtual bool muda::SubFieldImpl< FieldEntryLayout::SoA >::allow_inplace_shrink () const
```



Implements [*muda::SubFieldInterface::allow\_inplace\_shrink*](classmuda_1_1_sub_field_interface.md#function-allow_inplace_shrink)


<hr>



### function build\_impl 

```C++
virtual void muda::SubFieldImpl< FieldEntryLayout::SoA >::build_impl () override
```



Implements [*muda::SubFieldInterface::build\_impl*](classmuda_1_1_sub_field_interface.md#function-build_impl)


<hr>



### function calculate\_new\_cores 

```C++
virtual void muda::SubFieldImpl< FieldEntryLayout::SoA >::calculate_new_cores (
    std::byte * byte_buffer,
    size_t total_bytes,
    size_t element_count,
    span< FieldEntryCore > new_cores
) override
```



Implements [*muda::SubFieldInterface::calculate\_new\_cores*](classmuda_1_1_sub_field_interface.md#function-calculate_new_cores)


<hr>



### function require\_total\_buffer\_byte\_size 

```C++
virtual size_t muda::SubFieldImpl< FieldEntryLayout::SoA >::require_total_buffer_byte_size (
    size_t element_count
) override
```



Implements [*muda::SubFieldInterface::require\_total\_buffer\_byte\_size*](classmuda_1_1_sub_field_interface.md#function-require_total_buffer_byte_size)


<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/sub_field/soa_sub_field.h`

