

# Class muda::Field



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Field**](classmuda_1_1_field.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef FieldEntryLayout | [**Layout**](#typedef-layout)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Field**](#function-field) () <br> |
|  size\_t | [**num\_sub\_fields**](#function-num_sub_fields) () const<br> |
|  [**SubField**](classmuda_1_1_sub_field.md) & | [**operator[]**](#function-operator) (std::string\_view name) <br> |
|   | [**~Field**](#function-field) () <br> |




























## Public Types Documentation




### typedef Layout 

```C++
using muda::Field::Layout =  FieldEntryLayout;
```




<hr>
## Public Functions Documentation




### function Field 

```C++
muda::Field::Field () 
```




<hr>



### function num\_sub\_fields 

```C++
inline size_t muda::Field::num_sub_fields () const
```




<hr>



### function operator[] 

```C++
SubField & muda::Field::operator[] (
    std::string_view name
) 
```




<hr>



### function ~Field 

```C++
muda::Field::~Field () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field.h`

