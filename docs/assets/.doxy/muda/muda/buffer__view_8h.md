

# File buffer\_view.h



[**FileList**](files.md) **>** [**buffer**](dir_9b44f68c181db0b11e9502e462454d05.md) **>** [**buffer\_view.h**](buffer__view_8h.md)

[Go to the source code of this file](buffer__view_8h_source.md)

_A view interface for any array-like liner memory, which can be constructed from DeviceBuffer/DeviceVector or any thing that is a array-like liner memory, e.g. raw cuda pointer._ [More...](#detailed-description)

* `#include <cuda.h>`
* `#include <cuda_runtime.h>`
* `#include <cuda_runtime_api.h>`
* `#include <cinttypes>`
* `#include <muda/type_traits/type_modifier.h>`
* `#include <muda/viewer/dense/dense_1d.h>`
* `#include <muda/buffer/buffer_fwd.h>`
* `#include <muda/view/view_base.h>`
* `#include "details/buffer_view.inl"`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**muda**](namespacemuda.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**BufferViewT**](classmuda_1_1_buffer_view_t.md) &lt;IsConst, typename T&gt;<br> |
| struct | [**read\_only\_viewer&lt; BufferView&lt; T &gt; &gt;**](structmuda_1_1read__only__viewer_3_01_buffer_view_3_01_t_01_4_01_4.md) &lt;typename T&gt;<br> |
| struct | [**read\_write\_viewer&lt; CBufferView&lt; T &gt; &gt;**](structmuda_1_1read__write__viewer_3_01_c_buffer_view_3_01_t_01_4_01_4.md) &lt;typename T&gt;<br> |


















































# Detailed Description




**Author:**

MuGdxy 




**Date:**

January 2024 





    

------------------------------
The documentation for this class was generated from the following file `src/muda/buffer/buffer_view.h`

