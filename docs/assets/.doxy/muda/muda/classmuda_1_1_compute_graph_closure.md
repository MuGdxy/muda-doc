

# Class muda::ComputeGraphClosure



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphClosure**](classmuda_1_1_compute_graph_closure.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  auto | [**clousure\_id**](#function-clousure_id) () const<br> |
|  span&lt; const [**ComputeGraphDependency**](classmuda_1_1_compute_graph_dependency.md) &gt; | [**deps**](#function-deps) () const<br> |
| virtual void | [**graphviz\_def**](#function-graphviz_def) (std::ostream & o, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
| virtual void | [**graphviz\_id**](#function-graphviz_id) (std::ostream & o, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
| virtual void | [**graphviz\_var\_usages**](#function-graphviz_var_usages) (std::ostream & o, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options) const<br> |
|  auto | [**name**](#function-name) () const<br> |
|  auto | [**type**](#function-type) () const<br> |
|  const auto & | [**var\_usages**](#function-var_usages) () const<br> |
| virtual  | [**~ComputeGraphClosure**](#function-computegraphclosure) () = default<br> |




## Protected Types

| Type | Name |
| ---: | :--- |
| typedef std::shared\_ptr&lt; T &gt; | [**S**](#typedef-s)  <br> |




## Protected Attributes

| Type | Name |
| ---: | :--- |
|  uint64\_t | [**m\_access\_graph\_index**](#variable-m_access_graph_index)  <br> |
|  std::function&lt; void()&gt; | [**m\_closure**](#variable-m_closure)  <br> |
|  [**ClosureId**](classmuda_1_1_closure_id.md) | [**m\_clousure\_id**](#variable-m_clousure_id)  <br> |
|  size\_t | [**m\_deps\_begin**](#variable-m_deps_begin)   = = 0<br> |
|  size\_t | [**m\_deps\_count**](#variable-m_deps_count)   = = 0<br> |
|  [**ComputeGraph**](classmuda_1_1_compute_graph.md) \* | [**m\_graph**](#variable-m_graph)  <br> |
|  std::vector&lt; [**ComputeGraphNodeBase**](classmuda_1_1_compute_graph_node_base.md) \* &gt; | [**m\_graph\_nodes**](#variable-m_graph_nodes)  <br> |
|  std::string | [**m\_name**](#variable-m_name)  <br> |
|  ComputeGraphNodeType | [**m\_type**](#variable-m_type)  <br> |
|  std::map&lt; [**VarId**](classmuda_1_1_var_id.md), ComputeGraphVarUsage &gt; | [**m\_var\_usages**](#variable-m_var_usages)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphClosure**](#function-computegraphclosure) ([**ComputeGraph**](classmuda_1_1_compute_graph.md) \* graph, [**ClosureId**](classmuda_1_1_closure_id.md) clousure\_id, std::string\_view name, const std::function&lt; void()&gt; f) <br> |
|  void | [**operator()**](#function-operator()) () <br> |
|  void | [**set\_deps\_range**](#function-set_deps_range) (size\_t begin, size\_t count) <br> |




## Public Functions Documentation




### function clousure\_id 

```C++
inline auto muda::ComputeGraphClosure::clousure_id () const
```




<hr>



### function deps 

```C++
span< const ComputeGraphDependency > muda::ComputeGraphClosure::deps () const
```




<hr>



### function graphviz\_def 

```C++
virtual void muda::ComputeGraphClosure::graphviz_def (
    std::ostream & o,
    const ComputeGraphGraphvizOptions & options
) const
```




<hr>



### function graphviz\_id 

```C++
virtual void muda::ComputeGraphClosure::graphviz_id (
    std::ostream & o,
    const ComputeGraphGraphvizOptions & options
) const
```




<hr>



### function graphviz\_var\_usages 

```C++
virtual void muda::ComputeGraphClosure::graphviz_var_usages (
    std::ostream & o,
    const ComputeGraphGraphvizOptions & options
) const
```




<hr>



### function name 

```C++
inline auto muda::ComputeGraphClosure::name () const
```




<hr>



### function type 

```C++
inline auto muda::ComputeGraphClosure::type () const
```




<hr>



### function var\_usages 

```C++
inline const auto & muda::ComputeGraphClosure::var_usages () const
```




<hr>



### function ~ComputeGraphClosure 

```C++
virtual muda::ComputeGraphClosure::~ComputeGraphClosure () = default
```




<hr>
## Protected Types Documentation




### typedef S 

```C++
using muda::ComputeGraphClosure::S =  std::shared_ptr<T>;
```




<hr>
## Protected Attributes Documentation




### variable m\_access\_graph\_index 

```C++
uint64_t muda::ComputeGraphClosure::m_access_graph_index;
```




<hr>



### variable m\_closure 

```C++
std::function<void()> muda::ComputeGraphClosure::m_closure;
```




<hr>



### variable m\_clousure\_id 

```C++
ClosureId muda::ComputeGraphClosure::m_clousure_id;
```




<hr>



### variable m\_deps\_begin 

```C++
size_t muda::ComputeGraphClosure::m_deps_begin;
```




<hr>



### variable m\_deps\_count 

```C++
size_t muda::ComputeGraphClosure::m_deps_count;
```




<hr>



### variable m\_graph 

```C++
ComputeGraph* muda::ComputeGraphClosure::m_graph;
```




<hr>



### variable m\_graph\_nodes 

```C++
std::vector<ComputeGraphNodeBase*> muda::ComputeGraphClosure::m_graph_nodes;
```




<hr>



### variable m\_name 

```C++
std::string muda::ComputeGraphClosure::m_name;
```




<hr>



### variable m\_type 

```C++
ComputeGraphNodeType muda::ComputeGraphClosure::m_type;
```




<hr>



### variable m\_var\_usages 

```C++
std::map<VarId, ComputeGraphVarUsage> muda::ComputeGraphClosure::m_var_usages;
```




<hr>
## Protected Functions Documentation




### function ComputeGraphClosure 

```C++
inline muda::ComputeGraphClosure::ComputeGraphClosure (
    ComputeGraph * graph,
    ClosureId clousure_id,
    std::string_view name,
    const std::function< void()> f
) 
```




<hr>



### function operator() 

```C++
inline void muda::ComputeGraphClosure::operator() () 
```




<hr>



### function set\_deps\_range 

```C++
void muda::ComputeGraphClosure::set_deps_range (
    size_t begin,
    size_t count
) 
```




<hr>## Friends Documentation





### friend ComputeGraphAccessor 

```C++
class muda::ComputeGraphClosure::ComputeGraphAccessor (
    details::ComputeGraphAccessor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_closure.h`

