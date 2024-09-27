

# Class muda::Event



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**Event**](classmuda_1_1_event.md)



_RAII wrapper for cudaEvent._ 

* `#include <event.h>`

















## Public Types

| Type | Name |
| ---: | :--- |
| enum unsigned int | [**Bit**](#enum-bit)  <br> |
| enum  | [**QueryResult**](#enum-queryresult)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Event**](#function-event-13) ([**Flags**](classmuda_1_1_flags.md)&lt; [**Bit**](classmuda_1_1_event.md#enum-bit) &gt; flag=Bit::eDisableTiming) <br> |
|   | [**Event**](#function-event-23) (const [**Event**](classmuda_1_1_event.md) &) = delete<br> |
|   | [**Event**](#function-event-33) ([**Event**](classmuda_1_1_event.md) && o) <br> |
|   | [**operator cudaEvent\_t**](#function-operator-cudaevent_t) () <br> |
|  [**Event**](classmuda_1_1_event.md) & | [**operator=**](#function-operator) (const [**Event**](classmuda_1_1_event.md) &) = delete<br> |
|  [**Event**](classmuda_1_1_event.md) & | [**operator=**](#function-operator_1) ([**Event**](classmuda_1_1_event.md) && o) <br> |
|  [**QueryResult**](classmuda_1_1_event.md#enum-queryresult) | [**query**](#function-query) () const<br> |
|  cudaEvent\_t | [**viewer**](#function-viewer) () const<br> |
|   | [**~Event**](#function-event) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  float | [**elapsed\_time**](#function-elapsed_time) (cudaEvent\_t start, cudaEvent\_t stop) <br> |


























## Public Types Documentation




### enum Bit 

```C++
enum muda::Event::Bit {
    eDefault = cudaEventDefault,
    eBlockingSync = cudaEventBlockingSync,
    eDisableTiming = cudaEventDisableTiming,
    eInterprocess = cudaEventInterprocess
};
```




<hr>



### enum QueryResult 

```C++
enum muda::Event::QueryResult {
    eFinished = cudaSuccess,
    eNotReady = cudaErrorNotReady
};
```




<hr>
## Public Functions Documentation




### function Event [1/3]

```C++
muda::Event::Event (
    Flags < Bit > flag=Bit::eDisableTiming
) 
```




<hr>



### function Event [2/3]

```C++
muda::Event::Event (
    const Event &
) = delete
```




<hr>



### function Event [3/3]

```C++
muda::Event::Event (
    Event && o
) 
```




<hr>



### function operator cudaEvent\_t 

```C++
inline muda::Event::operator cudaEvent_t () 
```




<hr>



### function operator= 

```C++
Event & muda::Event::operator= (
    const Event &
) = delete
```




<hr>



### function operator= 

```C++
Event & muda::Event::operator= (
    Event && o
) 
```




<hr>



### function query 

```C++
QueryResult muda::Event::query () const
```




<hr>



### function viewer 

```C++
inline cudaEvent_t muda::Event::viewer () const
```




<hr>



### function ~Event 

```C++
muda::Event::~Event () 
```




<hr>
## Public Static Functions Documentation




### function elapsed\_time 

```C++
static float muda::Event::elapsed_time (
    cudaEvent_t start,
    cudaEvent_t stop
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/launch/event.h`

