

# Class muda::details::MatrixFormatConverterBase



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**MatrixFormatConverterBase**](classmuda_1_1details_1_1_matrix_format_converter_base.md)










Inherited by the following classes: [muda::details::MatrixFormatConverter](classmuda_1_1details_1_1_matrix_format_converter.md),  [muda::details::MatrixFormatConverter&lt; T, 1 &gt;](classmuda_1_1details_1_1_matrix_format_converter_3_01_t_00_011_01_4.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MatrixFormatConverterBase**](#function-matrixformatconverterbase) ([**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & context, cudaDataType\_t data\_type, int N) <br> |
|  auto | [**cublas**](#function-cublas) () const<br> |
|  auto | [**cusolver\_dn**](#function-cusolver_dn) () const<br> |
|  auto | [**cusolver\_sp**](#function-cusolver_sp) () const<br> |
|  auto | [**cusparse**](#function-cusparse) () const<br> |
|  auto | [**data\_type**](#function-data_type) () const<br> |
|  auto | [**dim**](#function-dim) () const<br> |
|  void | [**loose\_resize**](#function-loose_resize) ([**DeviceBuffer**](classmuda_1_1_device_buffer.md)&lt; T &gt; & buf, size\_t new\_size) <br> |
| virtual  | [**~MatrixFormatConverterBase**](#function-matrixformatconverterbase) () = default<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_N**](#variable-m_n)  <br> |
|  cudaDataType\_t | [**m\_data\_type**](#variable-m_data_type)  <br> |
|  [**LinearSystemHandles**](classmuda_1_1_linear_system_handles.md) & | [**m\_handles**](#variable-m_handles)  <br> |




















## Public Functions Documentation




### function MatrixFormatConverterBase 

```C++
inline muda::details::MatrixFormatConverterBase::MatrixFormatConverterBase (
    LinearSystemHandles & context,
    cudaDataType_t data_type,
    int N
) 
```




<hr>



### function cublas 

```C++
inline auto muda::details::MatrixFormatConverterBase::cublas () const
```




<hr>



### function cusolver\_dn 

```C++
inline auto muda::details::MatrixFormatConverterBase::cusolver_dn () const
```




<hr>



### function cusolver\_sp 

```C++
inline auto muda::details::MatrixFormatConverterBase::cusolver_sp () const
```




<hr>



### function cusparse 

```C++
inline auto muda::details::MatrixFormatConverterBase::cusparse () const
```




<hr>



### function data\_type 

```C++
inline auto muda::details::MatrixFormatConverterBase::data_type () const
```




<hr>



### function dim 

```C++
inline auto muda::details::MatrixFormatConverterBase::dim () const
```




<hr>



### function loose\_resize 

```C++
template<typename T>
inline void muda::details::MatrixFormatConverterBase::loose_resize (
    DeviceBuffer < T > & buf,
    size_t new_size
) 
```




<hr>



### function ~MatrixFormatConverterBase 

```C++
virtual muda::details::MatrixFormatConverterBase::~MatrixFormatConverterBase () = default
```




<hr>
## Protected Attributes Documentation




### variable m\_N 

```C++
int muda::details::MatrixFormatConverterBase::m_N;
```




<hr>



### variable m\_data\_type 

```C++
cudaDataType_t muda::details::MatrixFormatConverterBase::m_data_type;
```




<hr>



### variable m\_handles 

```C++
LinearSystemHandles& muda::details::MatrixFormatConverterBase::m_handles;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/matrix_format_converter_impl.h`

