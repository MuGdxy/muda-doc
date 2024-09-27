

# Class muda::ComputeGraphBuilder



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphBuilder**](classmuda_1_1_compute_graph_builder.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**capture**](#function-capture-12) (CaptureAction && cap) <br> |
|  void | [**capture**](#function-capture-22) (std::string\_view name, CaptureAction && cap) <br> |
|  Phase | [**current\_phase**](#function-current_phase) () <br> |
|  void | [**invoke\_phase\_actions**](#function-invoke_phase_actions-13) (PhaseAction && do\_when\_direct\_launch, PhaseAction && do\_when\_set\_node, PhaseAction && do\_when\_topo\_building\_set\_node) <br> |
|  void | [**invoke\_phase\_actions**](#function-invoke_phase_actions-23) (PhaseAction && do\_when\_direct\_launch, PhaseAction && do\_when\_set\_node) <br> |
|  void | [**invoke\_phase\_actions**](#function-invoke_phase_actions-33) (PhaseAction && do\_in\_every\_phase) <br> |
|  bool | [**is\_building**](#function-is_building) () <br> |
|  bool | [**is\_caturing**](#function-is_caturing) () <br> |
|  bool | [**is\_direct\_launching**](#function-is_direct_launching) () <br> |
|  bool | [**is\_phase\_none**](#function-is_phase_none) () <br> |
|  bool | [**is\_phase\_serial\_launching**](#function-is_phase_serial_launching) () <br> |
|  bool | [**is\_topo\_building**](#function-is_topo_building) () <br> |


























## Public Static Functions Documentation




### function capture [1/2]

```C++
static void muda::ComputeGraphBuilder::capture (
    CaptureAction && cap
) 
```




<hr>



### function capture [2/2]

```C++
static void muda::ComputeGraphBuilder::capture (
    std::string_view name,
    CaptureAction && cap
) 
```




<hr>



### function current\_phase 

```C++
static Phase muda::ComputeGraphBuilder::current_phase () 
```




<hr>



### function invoke\_phase\_actions [1/3]

```C++
static void muda::ComputeGraphBuilder::invoke_phase_actions (
    PhaseAction && do_when_direct_launch,
    PhaseAction && do_when_set_node,
    PhaseAction && do_when_topo_building_set_node
) 
```




<hr>



### function invoke\_phase\_actions [2/3]

```C++
static void muda::ComputeGraphBuilder::invoke_phase_actions (
    PhaseAction && do_when_direct_launch,
    PhaseAction && do_when_set_node
) 
```




<hr>



### function invoke\_phase\_actions [3/3]

```C++
static void muda::ComputeGraphBuilder::invoke_phase_actions (
    PhaseAction && do_in_every_phase
) 
```




<hr>



### function is\_building 

```C++
static bool muda::ComputeGraphBuilder::is_building () 
```




<hr>



### function is\_caturing 

```C++
static bool muda::ComputeGraphBuilder::is_caturing () 
```




<hr>



### function is\_direct\_launching 

```C++
static bool muda::ComputeGraphBuilder::is_direct_launching () 
```




<hr>



### function is\_phase\_none 

```C++
static bool muda::ComputeGraphBuilder::is_phase_none () 
```




<hr>



### function is\_phase\_serial\_launching 

```C++
static bool muda::ComputeGraphBuilder::is_phase_serial_launching () 
```




<hr>



### function is\_topo\_building 

```C++
static bool muda::ComputeGraphBuilder::is_topo_building () 
```




<hr>## Friends Documentation





### friend ComputeGraphAccessor 

```C++
class muda::ComputeGraphBuilder::ComputeGraphAccessor (
    details::ComputeGraphAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_builder.h`

