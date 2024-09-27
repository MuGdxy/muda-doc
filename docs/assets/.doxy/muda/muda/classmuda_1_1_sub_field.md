

# Class muda::SubField



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**SubField**](classmuda_1_1_sub_field.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**FieldBuilder**](classmuda_1_1_field_builder.md)&lt; FieldEntryLayout::AoS &gt; | [**AoS**](#function-aos) (const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & options={}) <br>_The layout is array of structs (determined at compile time)_  |
|  [**FieldBuilder**](classmuda_1_1_field_builder.md)&lt; FieldEntryLayout::AoSoA &gt; | [**AoSoA**](#function-aosoa) (uint32\_t innermost\_array\_size=32, const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & options={}) <br>_The layout is array of structs of arrays (determined at compile time)_  |
|  [**FieldBuilder**](classmuda_1_1_field_builder.md)&lt; FieldEntryLayout::SoA &gt; | [**SoA**](#function-soa) (const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & options={}) <br>_The layout is struct of arrays (determined at compile time)_  |
|   | [**SubField**](#function-subfield-24) ([**Field**](classmuda_1_1_field.md) & field, std::string\_view name) <br> |
|   | [**SubField**](#function-subfield-34) (const [**SubField**](classmuda_1_1_sub_field.md) &) = delete<br> |
|   | [**SubField**](#function-subfield-44) ([**SubField**](classmuda_1_1_sub_field.md) &&) = delete<br> |
|  [**FieldBuilder**](classmuda_1_1_field_builder.md)&lt; Layout &gt; | [**builder**](#function-builder-12) ([**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) layout=[**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md){Layout}, const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & options={}) <br> |
|  [**FieldBuilder**](classmuda_1_1_field_builder.md)&lt; FieldEntryLayout::RuntimeLayout &gt; | [**builder**](#function-builder-22) ([**FieldEntryLayoutInfo**](classmuda_1_1_field_entry_layout_info.md) layout, const [**FieldBuildOptions**](classmuda_1_1_field_build_options.md) & options={}) <br>_The layout is determined at runtime._  |
|  std::string\_view | [**name**](#function-name) () const<br> |
|  [**SubField**](classmuda_1_1_sub_field.md) & | [**operator=**](#function-operator) (const [**SubField**](classmuda_1_1_sub_field.md) &) = delete<br> |
|  [**SubField**](classmuda_1_1_sub_field.md) & | [**operator=**](#function-operator_1) ([**SubField**](classmuda_1_1_sub_field.md) &&) = delete<br> |
|  void | [**resize**](#function-resize) (size\_t num\_elements) <br> |
|  size\_t | [**size**](#function-size) () const<br> |
|   | [**~SubField**](#function-subfield) () <br> |




























## Public Functions Documentation




### function AoS 

_The layout is array of structs (determined at compile time)_ 
```C++
FieldBuilder < FieldEntryLayout::AoS > muda::SubField::AoS (
    const FieldBuildOptions & options={}
) 
```





**Returns:**







        

<hr>



### function AoSoA 

_The layout is array of structs of arrays (determined at compile time)_ 
```C++
FieldBuilder < FieldEntryLayout::AoSoA > muda::SubField::AoSoA (
    uint32_t innermost_array_size=32,
    const FieldBuildOptions & options={}
) 
```





**Parameters:**


* `layout` 



**Returns:**







        

<hr>



### function SoA 

_The layout is struct of arrays (determined at compile time)_ 
```C++
FieldBuilder < FieldEntryLayout::SoA > muda::SubField::SoA (
    const FieldBuildOptions & options={}
) 
```





**Returns:**







        

<hr>



### function SubField [2/4]

```C++
muda::SubField::SubField (
    Field & field,
    std::string_view name
) 
```




<hr>



### function SubField [3/4]

```C++
muda::SubField::SubField (
    const SubField &
) = delete
```




<hr>



### function SubField [4/4]

```C++
muda::SubField::SubField (
    SubField &&
) = delete
```




<hr>



### function builder [1/2]

```C++
template<FieldEntryLayout Layout>
FieldBuilder < Layout > muda::SubField::builder (
    FieldEntryLayoutInfo layout=FieldEntryLayoutInfo {Layout},
    const FieldBuildOptions & options={}
) 
```




<hr>



### function builder [2/2]

_The layout is determined at runtime._ 
```C++
FieldBuilder < FieldEntryLayout::RuntimeLayout > muda::SubField::builder (
    FieldEntryLayoutInfo layout,
    const FieldBuildOptions & options={}
) 
```





**Parameters:**


* `layout` 



**Returns:**







        

<hr>



### function name 

```C++
inline std::string_view muda::SubField::name () const
```




<hr>



### function operator= 

```C++
SubField & muda::SubField::operator= (
    const SubField &
) = delete
```




<hr>



### function operator= 

```C++
SubField & muda::SubField::operator= (
    SubField &&
) = delete
```




<hr>



### function resize 

```C++
void muda::SubField::resize (
    size_t num_elements
) 
```




<hr>



### function size 

```C++
size_t muda::SubField::size () const
```




<hr>



### function ~SubField 

```C++
muda::SubField::~SubField () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/sub_field.h`

