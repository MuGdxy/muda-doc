

# Class muda::ComputeGraphVarBase



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md)










Inherited by the following classes: [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md),  [muda::ComputeGraphVar](classmuda_1_1_compute_graph_var.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**graphviz\_def**](#function-graphviz_def) (std::ostream & os, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
| virtual void | [**graphviz\_id**](#function-graphviz_id) (std::ostream & os, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
|  bool | [**is\_using**](#function-is_using) () <br> |
|  bool | [**is\_valid**](#function-is_valid) () const<br> |
|  std::string\_view | [**name**](#function-name) () const<br> |
|  [**Event::QueryResult**](classmuda_1_1_event.md#enum-queryresult) | [**query**](#function-query) () <br> |
|  void | [**sync**](#function-sync) () <br> |
|  void | [**update**](#function-update) () <br> |
|  [**VarId**](classmuda_1_1_var_id.md) | [**var\_id**](#function-var_id) () const<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  std::set&lt; [**ClosureId**](classmuda_1_1_closure_id.md) &gt; | [**m\_closure\_ids**](#variable-m_closure_ids)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphVarBase**](#function-computegraphvarbase-12) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id) <br> |
|   | [**ComputeGraphVarBase**](#function-computegraphvarbase-22) ([**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md) \* var\_manager, std::string\_view name, [**VarId**](classmuda_1_1_var_id.md) var\_id, bool is\_valid) <br> |
|  ROView | [**\_ceval**](#function-_ceval) (ROView & view) const<br> |
|  RWView | [**\_eval**](#function-_eval) (const RWView & view) <br> |
|  void | [**base\_update**](#function-base_update) () <br> |
| virtual  | [**~ComputeGraphVarBase**](#function-computegraphvarbase) () = default<br> |




## Public Functions Documentation




### function graphviz\_def 

```C++
virtual void muda::ComputeGraphVarBase::graphviz_def (
    std::ostream & os,
    const ComputeGraphGraphvizOptions & options
) const
```




<hr>



### function graphviz\_id 

```C++
virtual void muda::ComputeGraphVarBase::graphviz_id (
    std::ostream & os,
    const ComputeGraphGraphvizOptions & options
) const
```




<hr>



### function is\_using 

```C++
bool muda::ComputeGraphVarBase::is_using () 
```




<hr>



### function is\_valid 

```C++
inline bool muda::ComputeGraphVarBase::is_valid () const
```




<hr>



### function name 

```C++
inline std::string_view muda::ComputeGraphVarBase::name () const
```




<hr>



### function query 

```C++
Event::QueryResult muda::ComputeGraphVarBase::query () 
```




<hr>



### function sync 

```C++
void muda::ComputeGraphVarBase::sync () 
```




<hr>



### function update 

```C++
void muda::ComputeGraphVarBase::update () 
```




<hr>



### function var\_id 

```C++
inline VarId muda::ComputeGraphVarBase::var_id () const
```




<hr>
## Protected Attributes Documentation




### variable m\_closure\_ids 

```C++
std::set<ClosureId> muda::ComputeGraphVarBase::m_closure_ids;
```




<hr>
## Protected Functions Documentation




### function ComputeGraphVarBase [1/2]

```C++
inline muda::ComputeGraphVarBase::ComputeGraphVarBase (
    ComputeGraphVarManager * var_manager,
    std::string_view name,
    VarId var_id
) 
```




<hr>



### function ComputeGraphVarBase [2/2]

```C++
inline muda::ComputeGraphVarBase::ComputeGraphVarBase (
    ComputeGraphVarManager * var_manager,
    std::string_view name,
    VarId var_id,
    bool is_valid
) 
```




<hr>



### function \_ceval 

```C++
template<typename ROView>
ROView muda::ComputeGraphVarBase::_ceval (
    ROView & view
) const
```




<hr>



### function \_eval 

```C++
template<typename RWView>
RWView muda::ComputeGraphVarBase::_eval (
    const RWView & view
) 
```




<hr>



### function base\_update 

```C++
void muda::ComputeGraphVarBase::base_update () 
```




<hr>



### function ~ComputeGraphVarBase 

```C++
virtual muda::ComputeGraphVarBase::~ComputeGraphVarBase () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_var.h`

