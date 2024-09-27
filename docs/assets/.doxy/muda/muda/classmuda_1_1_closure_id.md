

# Class muda::ClosureId



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ClosureId**](classmuda_1_1_closure_id.md)








Inherits the following classes: [muda::IdWithType](classmuda_1_1_id_with_type.md)
















## Public Types inherited from muda::IdWithType

See [muda::IdWithType](classmuda_1_1_id_with_type.md)

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](classmuda_1_1_id_with_type.md#typedef-value_type)  <br> |












## Public Static Attributes inherited from muda::IdWithType

See [muda::IdWithType](classmuda_1_1_id_with_type.md)

| Type | Name |
| ---: | :--- |
|  constexpr auto | [**invalid\_id**](classmuda_1_1_id_with_type.md#variable-invalid_id)   = = std::numeric\_limits&lt;value\_type&gt;::max()<br> |




























## Public Functions inherited from muda::IdWithType

See [muda::IdWithType](classmuda_1_1_id_with_type.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**IdWithType**](classmuda_1_1_id_with_type.md#function-idwithtype-12) (value\_type value) noexcept<br> |
|  MUDA\_GENERIC | [**IdWithType**](classmuda_1_1_id_with_type.md#function-idwithtype-22) () noexcept<br> |
|  MUDA\_GENERIC bool | [**is\_valid**](classmuda_1_1_id_with_type.md#function-is_valid) () noexcept const<br> |
|  MUDA\_GENERIC value\_type | [**value**](classmuda_1_1_id_with_type.md#function-value) () noexcept const<br> |
















## Protected Attributes inherited from muda::IdWithType

See [muda::IdWithType](classmuda_1_1_id_with_type.md)

| Type | Name |
| ---: | :--- |
|  value\_type | [**m\_value**](classmuda_1_1_id_with_type.md#variable-m_value)   = {invalid\_id}<br> |







































------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_closure_id.h`

