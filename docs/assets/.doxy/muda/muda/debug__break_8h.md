

# File debug\_break.h



[**FileList**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**debug\_break.h**](debug__break_8h.md)

[Go to the source code of this file](debug__break_8h_source.md)



* `#include <signal.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**\_\_attribute\_\_**](#function-__attribute__) ((always\_inline)) <br> |



























## Macros

| Type | Name |
| ---: | :--- |
| define  | [**DEBUG\_BREAK\_IMPL**](debug__break_8h.md#define-debug_break_impl)  DEBUG\_BREAK\_USE\_SIGTRAP<br> |
| define  | [**DEBUG\_BREAK\_USE\_BULTIN\_TRAP**](debug__break_8h.md#define-debug_break_use_bultin_trap)  2<br> |
| define  | [**DEBUG\_BREAK\_USE\_SIGTRAP**](debug__break_8h.md#define-debug_break_use_sigtrap)  3<br> |
| define  | [**DEBUG\_BREAK\_USE\_TRAP\_INSTRUCTION**](debug__break_8h.md#define-debug_break_use_trap_instruction)  1<br> |

## Public Functions Documentation




### function \_\_attribute\_\_ 

```C++
__attribute__ (
    (always_inline)
) 
```




<hr>
## Macro Definition Documentation





### define DEBUG\_BREAK\_IMPL 

```C++
#define DEBUG_BREAK_IMPL DEBUG_BREAK_USE_SIGTRAP
```




<hr>



### define DEBUG\_BREAK\_USE\_BULTIN\_TRAP 

```C++
#define DEBUG_BREAK_USE_BULTIN_TRAP 2
```




<hr>



### define DEBUG\_BREAK\_USE\_SIGTRAP 

```C++
#define DEBUG_BREAK_USE_SIGTRAP 3
```




<hr>



### define DEBUG\_BREAK\_USE\_TRAP\_INSTRUCTION 

```C++
#define DEBUG_BREAK_USE_TRAP_INSTRUCTION 1
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/tools/debug_break.h`

