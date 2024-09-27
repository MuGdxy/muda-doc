

# File sparse\_spatial\_hash\_impl.h



[**FileList**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**geo**](dir_e05e4ae50bce28830f3a7b1d7f2eeff2.md) **>** [**spatial\_hash**](dir_58b30d2a266b6e98a9cbea81c385691b.md) **>** [**sparse\_spatial\_hash\_impl.h**](sparse__spatial__hash__impl_8h.md)

[Go to the source code of this file](sparse__spatial__hash__impl_8h_source.md)



* `#include <muda/muda_def.h>`
* `#include <muda/ext/geo/spatial_hash/morton_hash.h>`
* `#include <muda/launch/launch.h>`
* `#include <muda/launch/parallel_for.h>`
* `#include <muda/buffer/device_buffer.h>`
* `#include <muda/ext/geo/spatial_hash/bounding_volume.h>`
* `#include <muda/ext/geo/spatial_hash/collision_pair.h>`
* `#include "details/sparse_spatial_hash_impl.inl"`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |
| namespace | [**spatial\_hash**](namespacemuda_1_1spatial__hash.md) <br> |
| namespace | [**details**](namespacemuda_1_1spatial__hash_1_1details.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**SpatialHashTableInfo**](classmuda_1_1spatial__hash_1_1_spatial_hash_table_info.md) &lt;typename Hash&gt;<br> |
| class | [**SpatialPartitionCell**](classmuda_1_1spatial__hash_1_1_spatial_partition_cell.md) <br>_To represent a cell-object pair in the spatial hash 3D grid e.g. (cell\_id,object\_id) = (1024, 32) for the meaning: the 32th object overlap with the 1024th cell._  |
| class | [**SparseSpatialHashImpl**](classmuda_1_1spatial__hash_1_1details_1_1_sparse_spatial_hash_impl.md) &lt;typename Hash&gt;<br> |



















































------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/spatial_hash/sparse_spatial_hash_impl.h`

