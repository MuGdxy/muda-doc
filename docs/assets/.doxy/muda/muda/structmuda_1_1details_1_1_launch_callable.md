

# Struct muda::details::LaunchCallable

**template &lt;typename F&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**LaunchCallable**](structmuda_1_1details_1_1_launch_callable.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  F | [**callable**](#variable-callable)  <br> |
|  dim3 | [**dim**](#variable-dim)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**LaunchCallable**](#function-launchcallable) (U && f, const dim3 & d) <br> |




























## Public Attributes Documentation




### variable callable 

```C++
F muda::details::LaunchCallable< F >::callable;
```




<hr>



### variable dim 

```C++
dim3 muda::details::LaunchCallable< F >::dim;
```




<hr>
## Public Functions Documentation




### function LaunchCallable 

```C++
template<typename U>
inline muda::details::LaunchCallable::LaunchCallable (
    U && f,
    const dim3 & d
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/launch.h`

