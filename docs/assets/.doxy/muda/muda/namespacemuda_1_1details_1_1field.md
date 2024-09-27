

# Namespace muda::details::field



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**field**](namespacemuda_1_1details_1_1field.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::Stride&lt; Eigen::Dynamic, Eigen::Dynamic &gt; | [**MatStride**](#typedef-matstride)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC MatStride | [**make\_stride**](#function-make_stride) (const [**FieldEntryCore**](classmuda_1_1_field_entry_core.md) & core) <br> |




























## Public Types Documentation




### typedef MatStride 

```C++
using muda::details::field::MatStride = typedef Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic>;
```




<hr>
## Public Functions Documentation




### function make\_stride 

```C++
template<typename T, FieldEntryLayout Layout, int M, int N>
MUDA_GENERIC MatStride muda::details::field::make_stride (
    const FieldEntryCore & core
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/field/field_entry_viewer.h`

