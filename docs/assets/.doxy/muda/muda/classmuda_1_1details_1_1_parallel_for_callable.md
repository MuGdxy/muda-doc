

# Class muda::details::ParallelForCallable

**template &lt;typename F&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**details**](namespacemuda_1_1details.md) **>** [**ParallelForCallable**](classmuda_1_1details_1_1_parallel_for_callable.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  F | [**callable**](#variable-callable)  <br> |
|  int | [**count**](#variable-count)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**ParallelForCallable**](#function-parallelforcallable) (U && callable, int count) <br> |




























## Public Attributes Documentation




### variable callable 

```C++
F muda::details::ParallelForCallable< F >::callable;
```




<hr>



### variable count 

```C++
int muda::details::ParallelForCallable< F >::count;
```




<hr>
## Public Functions Documentation




### function ParallelForCallable 

```C++
template<typename U>
inline MUDA_GENERIC muda::details::ParallelForCallable::ParallelForCallable (
    U && callable,
    int count
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/parallel_for.h`

