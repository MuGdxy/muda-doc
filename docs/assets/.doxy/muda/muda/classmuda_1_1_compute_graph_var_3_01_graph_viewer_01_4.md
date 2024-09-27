

# Class muda::ComputeGraphVar&lt; GraphViewer &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphVar&lt; GraphViewer &gt;**](classmuda_1_1_compute_graph_var_3_01_graph_viewer_01_4.md)








Inherits the following classes: [muda::ComputeGraphVarBase](classmuda_1_1_compute_graph_var_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**GraphViewer**](classmuda_1_1_graph_viewer.md) | [**ROView**](#typedef-roview)  <br> |
| typedef [**GraphViewer**](classmuda_1_1_graph_viewer.md) | [**RWView**](#typedef-rwview)  <br> |








































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**ROView**](classmuda_1_1_graph_viewer.md) | [**ceval**](#function-ceval) () const<br> |
|  [**RWView**](classmuda_1_1_graph_viewer.md) | [**eval**](#function-eval) () <br> |
| virtual void | [**graphviz\_def**](#function-graphviz_def) (std::ostream & o, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) override const<br> |
|   | [**operator ROView**](#function-operator-roview) () const<br> |
|   | [**operator RWView**](#function-operator-rwview) () <br> |
|  [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; [**GraphViewer**](classmuda_1_1_graph_viewer.md) &gt; & | [**operator=**](#function-operator) (const [**RWView**](classmuda_1_1_graph_viewer.md) & view) <br> |
|  void | [**update**](#function-update) (const [**RWView**](classmuda_1_1_graph_viewer.md) & view) <br> |


## Public Functions inherited from muda::ComputeGraphVarBase

See [muda::ComputeGraphVarBase](classmuda_1_1_compute_graph_var_base.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**graphviz\_def**](classmuda_1_1_compute_graph_var_base.md#function-graphviz_def) (std::ostream & os, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
| virtual void | [**graphviz\_id**](classmuda_1_1_compute_graph_var_base.md#function-graphviz_id) (std::ostream & os, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
|  bool | [**is\_using**](classmuda_1_1_compute_graph_var_base.md#function-is_using) () <br> |
|  bool | [**is\_valid**](classmuda_1_1_compute_graph_var_base.md#function-is_valid) () const<br> |
|  std::string\_view | [**name**](classmuda_1_1_compute_graph_var_base.md#function-name) () const<br> |
|  [**Event::QueryResult**](classmuda_1_1_event.md#enum-queryresult) | [**query**](classmuda_1_1_compute_graph_var_base.md#function-query) () <br> |
|  void | [**sync**](classmuda_1_1_compute_graph_var_base.md#function-sync) () <br> |
|  void | [**update**](classmuda_1_1_compute_graph_var_base.md#function-update) () <br> |
|  [**VarId**](classmuda_1_1_var_id.md) | [**var\_id**](classmuda_1_1_compute_graph_var_base.md#function-var_id) () const<br> |
















## Protected Attributes inherited from muda::ComputeGraphVarBase

See [muda::ComputeGraphVarBase](classmuda_1_1_compute_graph_var_base.md)

| Type | Name |
| ---: | :--- |
|  std::set&lt; [**ClosureId**](classmuda_1_1_closure_id.md) &gt; | [**m\_closure\_ids**](classmuda_1_1_compute_graph_var_base.md#variable-m_closure_ids)  <br> |






























## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphVar**](#function-computegraphvar-12) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id) <br> |
|   | [**ComputeGraphVar**](#function-computegraphvar-22) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id, const [**RWView**](classmuda_1_1_graph_viewer.md) & init\_value) <br> |
|   | [**ComputeGraphVarBase**](#function-computegraphvarbase-12) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id) <br> |
|   | [**ComputeGraphVarBase**](#function-computegraphvarbase-22) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id, bool is\_valid) <br> |
| virtual  | [**~ComputeGraphVar**](#function-computegraphvar) () = default<br> |


## Protected Functions inherited from muda::ComputeGraphVarBase

See [muda::ComputeGraphVarBase](classmuda_1_1_compute_graph_var_base.md)

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md#function-computegraphvarbase-12) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id) <br> |
|   | [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md#function-computegraphvarbase-22) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id, bool is\_valid) <br> |
|  ROView | [**\_ceval**](classmuda_1_1_compute_graph_var_base.md#function-_ceval) (ROView & view) const<br> |
|  RWView | [**\_eval**](classmuda_1_1_compute_graph_var_base.md#function-_eval) (const RWView & view) <br> |
|  void | [**base\_update**](classmuda_1_1_compute_graph_var_base.md#function-base_update) () <br> |
| virtual  | [**~ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md#function-computegraphvarbase) () = default<br> |






## Public Types Documentation




### typedef ROView 

```C++
using muda::ComputeGraphVar< GraphViewer >::ROView =  GraphViewer;
```




<hr>



### typedef RWView 

```C++
using muda::ComputeGraphVar< GraphViewer >::RWView =  GraphViewer;
```




<hr>
## Public Functions Documentation




### function ceval 

```C++
inline ROView muda::ComputeGraphVar< GraphViewer >::ceval () const
```




<hr>



### function eval 

```C++
inline RWView muda::ComputeGraphVar< GraphViewer >::eval () 
```




<hr>



### function graphviz\_def 

```C++
virtual void muda::ComputeGraphVar< GraphViewer >::graphviz_def (
    std::ostream & o,
    const ComputeGraphGraphvizOptions & options
) override const
```



Implements [*muda::ComputeGraphVarBase::graphviz\_def*](classmuda_1_1_compute_graph_var_base.md#function-graphviz_def)


<hr>



### function operator ROView 

```C++
inline muda::ComputeGraphVar< GraphViewer >::operator ROView () const
```




<hr>



### function operator RWView 

```C++
inline muda::ComputeGraphVar< GraphViewer >::operator RWView () 
```




<hr>



### function operator= 

```C++
ComputeGraphVar < GraphViewer > & muda::ComputeGraphVar< GraphViewer >::operator= (
    const RWView & view
) 
```




<hr>



### function update 

```C++
void muda::ComputeGraphVar< GraphViewer >::update (
    const RWView & view
) 
```




<hr>
## Protected Functions Documentation




### function ComputeGraphVar [1/2]

```C++
inline muda::ComputeGraphVar< GraphViewer >::ComputeGraphVar (
    ComputeGraphVarManager * var_manager,
    std::string_view name,
    VarId var_id
) 
```




<hr>



### function ComputeGraphVar [2/2]

```C++
inline muda::ComputeGraphVar< GraphViewer >::ComputeGraphVar (
    ComputeGraphVarManager * var_manager,
    std::string_view name,
    VarId var_id,
    const RWView & init_value
) 
```




<hr>



### function ComputeGraphVarBase [1/2]

```C++
inline muda::ComputeGraphVar< GraphViewer >::ComputeGraphVarBase (
    ComputeGraphVarManager * var_manager,
    std::string_view name,
    VarId var_id
) 
```




<hr>



### function ComputeGraphVarBase [2/2]

```C++
inline muda::ComputeGraphVar< GraphViewer >::ComputeGraphVarBase (
    ComputeGraphVarManager * var_manager,
    std::string_view name,
    VarId var_id,
    bool is_valid
) 
```




<hr>



### function ~ComputeGraphVar 

```C++
virtual muda::ComputeGraphVar< GraphViewer >::~ComputeGraphVar () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/graph_graph_viewer.h`

