

# Class muda::FieldBuilder::EntryProxy



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**FieldBuilder**](classmuda_1_1_field_builder.md) **>** [**EntryProxy**](classmuda_1_1_field_builder_1_1_entry_proxy.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**EntryProxy**](#function-entryproxy) ([**FieldBuilder**](classmuda_1_1_field_builder.md)&lt; Layout &gt; & builder, std::string\_view name) <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, M, N &gt; & | [**matrix**](#function-matrix) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 2, 2 &gt; & | [**matrix2x2**](#function-matrix2x2) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 3, 3 &gt; & | [**matrix3x3**](#function-matrix3x3) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 4, 4 &gt; & | [**matrix4x4**](#function-matrix4x4) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 1, 1 &gt; & | [**scalar**](#function-scalar) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, N, 1 &gt; & | [**vector**](#function-vector) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 2, 1 &gt; & | [**vector2**](#function-vector2) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 3, 1 &gt; & | [**vector3**](#function-vector3) () <br> |
|  [**FieldEntry**](classmuda_1_1_field_entry.md)&lt; T, Layout, 4, 1 &gt; & | [**vector4**](#function-vector4) () <br> |




























## Public Functions Documentation




### function EntryProxy 

```C++
inline muda::FieldBuilder::EntryProxy::EntryProxy (
    FieldBuilder < Layout > & builder,
    std::string_view name
) 
```




<hr>



### function matrix 

```C++
template<typename T, int M, int N>
FieldEntry < T, Layout, M, N > & muda::FieldBuilder::EntryProxy::matrix () 
```




<hr>



### function matrix2x2 

```C++
template<typename T>
FieldEntry < T, Layout, 2, 2 > & muda::FieldBuilder::EntryProxy::matrix2x2 () 
```




<hr>



### function matrix3x3 

```C++
template<typename T>
FieldEntry < T, Layout, 3, 3 > & muda::FieldBuilder::EntryProxy::matrix3x3 () 
```




<hr>



### function matrix4x4 

```C++
template<typename T>
FieldEntry < T, Layout, 4, 4 > & muda::FieldBuilder::EntryProxy::matrix4x4 () 
```




<hr>



### function scalar 

```C++
template<typename T>
FieldEntry < T, Layout, 1, 1 > & muda::FieldBuilder::EntryProxy::scalar () 
```




<hr>



### function vector 

```C++
template<typename T, int N>
FieldEntry < T, Layout, N, 1 > & muda::FieldBuilder::EntryProxy::vector () 
```




<hr>



### function vector2 

```C++
template<typename T>
FieldEntry < T, Layout, 2, 1 > & muda::FieldBuilder::EntryProxy::vector2 () 
```




<hr>



### function vector3 

```C++
template<typename T>
FieldEntry < T, Layout, 3, 1 > & muda::FieldBuilder::EntryProxy::vector3 () 
```




<hr>



### function vector4 

```C++
template<typename T>
FieldEntry < T, Layout, 4, 1 > & muda::FieldBuilder::EntryProxy::vector4 () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_builder.h`

