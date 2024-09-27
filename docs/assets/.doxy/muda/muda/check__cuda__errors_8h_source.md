

# File check\_cuda\_errors.h

[**File List**](files.md) **>** [**check**](dir_3ada5fb1291f7068cec99adbe813154e.md) **>** [**check\_cuda\_errors.h**](check__cuda__errors_8h.md)

[Go to the documentation of this file](check__cuda__errors_8h.md)


```C++
#pragma once
#include <muda/check/check.h>
#define checkCudaErrors(val) ::muda::check((val), #val, __FILE__, __LINE__)
```


