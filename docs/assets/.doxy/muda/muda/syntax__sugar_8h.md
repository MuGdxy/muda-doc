

# File syntax\_sugar.h



[**FileList**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**syntax\_sugar.h**](syntax__sugar_8h.md)

[Go to the source code of this file](syntax__sugar_8h_source.md)



































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**MUDA\_DEVICE**](syntax__sugar_8h.md#define-muda_device) (\_\_VA\_ARGS\_\_) mutable<br> |
| define  | [**def**](syntax__sugar_8h.md#define-def) (viewer, from) viewer = (from).name(#viewer)<br> |
| define  | [**kernel\_name**](syntax__sugar_8h.md#define-kernel_name) () kernel\_name(\_\_FUNCTION\_\_)<br> |
| define  | [**node**](syntax__sugar_8h.md#define-node) (name) create\_node(name) &lt;&lt; [&]<br> |

## Macro Definition Documentation





### define MUDA\_DEVICE 

```C++
#define MUDA_DEVICE (
    __VA_ARGS__
) mutable
```




<hr>



### define def 

```C++
#define def (
    viewer,
    from
) viewer = (from).name(#viewer)
```




<hr>



### define kernel\_name 

```C++
#define kernel_name (
    
) kernel_name(__FUNCTION__)
```




<hr>



### define node 

```C++
#define node (
    name
) create_node(name) << [&]
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/syntax_sugar.h`

