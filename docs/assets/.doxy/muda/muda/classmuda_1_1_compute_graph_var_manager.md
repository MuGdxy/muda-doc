

# Class muda::ComputeGraphVarManager



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**ComputeGraphVarManager**](classmuda_1_1_compute_graph_var_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ComputeGraphVarManager**](#function-computegraphvarmanager) () = default<br> |
|  S&lt; [**ComputeGraph**](classmuda_1_1_compute_graph.md) &gt; | [**create\_graph**](#function-create_graph) (std::string\_view name="graph", ComputeGraphFlag flags={}) <br> |
|  [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; & | [**create\_var**](#function-create_var-12) (std::string\_view name) <br> |
|  [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; & | [**create\_var**](#function-create_var-22) (std::string\_view name, const T & init\_value) <br> |
|  [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; \* | [**find\_var**](#function-find_var) (std::string\_view name) <br> |
|  const auto & | [**graphs**](#function-graphs) () const<br> |
|  void | [**graphviz**](#function-graphviz) (std::ostream & os, const [**ComputeGraphGraphvizOptions**](classmuda_1_1_compute_graph_graphviz_options.md) & options={}) const<br> |
|  bool | [**is\_using**](#function-is_using-13) () const<br> |
|  bool | [**is\_using**](#function-is_using-23) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; &... vars) const<br> |
|  bool | [**is\_using**](#function-is_using-33) (const span&lt; const [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; vars) const<br> |
|  void | [**sync**](#function-sync-13) () const<br> |
|  void | [**sync**](#function-sync-23) (const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; &... vars) const<br> |
|  void | [**sync**](#function-sync-33) (const span&lt; const [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; vars) const<br> |
|  void | [**sync\_on**](#function-sync_on-13) (cudaStream\_t stream) const<br> |
|  void | [**sync\_on**](#function-sync_on-23) (cudaStream\_t stream, const [**ComputeGraphVar**](classmuda_1_1_compute_graph_var.md)&lt; T &gt; &... vars) const<br> |
|  void | [**sync\_on**](#function-sync_on-33) (cudaStream\_t stream, const span&lt; const [**ComputeGraphVarBase**](classmuda_1_1_compute_graph_var_base.md) \* &gt; vars) const<br> |
|   | [**~ComputeGraphVarManager**](#function-computegraphvarmanager) () <br> |




























## Public Functions Documentation




### function ComputeGraphVarManager 

```C++
muda::ComputeGraphVarManager::ComputeGraphVarManager () = default
```




<hr>



### function create\_graph 

```C++
S< ComputeGraph > muda::ComputeGraphVarManager::create_graph (
    std::string_view name="graph",
    ComputeGraphFlag flags={}
) 
```




<hr>



### function create\_var [1/2]

```C++
template<typename T>
ComputeGraphVar < T > & muda::ComputeGraphVarManager::create_var (
    std::string_view name
) 
```




<hr>



### function create\_var [2/2]

```C++
template<typename T>
ComputeGraphVar < T > & muda::ComputeGraphVarManager::create_var (
    std::string_view name,
    const T & init_value
) 
```




<hr>



### function find\_var 

```C++
template<typename T>
ComputeGraphVar < T > * muda::ComputeGraphVarManager::find_var (
    std::string_view name
) 
```




<hr>



### function graphs 

```C++
inline const auto & muda::ComputeGraphVarManager::graphs () const
```




<hr>



### function graphviz 

```C++
void muda::ComputeGraphVarManager::graphviz (
    std::ostream & os,
    const ComputeGraphGraphvizOptions & options={}
) const
```




<hr>



### function is\_using [1/3]

```C++
bool muda::ComputeGraphVarManager::is_using () const
```




<hr>



### function is\_using [2/3]

```C++
template<typename... T>
bool muda::ComputeGraphVarManager::is_using (
    const ComputeGraphVar < T > &... vars
) const
```




<hr>



### function is\_using [3/3]

```C++
bool muda::ComputeGraphVarManager::is_using (
    const span< const ComputeGraphVarBase * > vars
) const
```




<hr>



### function sync [1/3]

```C++
void muda::ComputeGraphVarManager::sync () const
```




<hr>



### function sync [2/3]

```C++
template<typename... T>
void muda::ComputeGraphVarManager::sync (
    const ComputeGraphVar < T > &... vars
) const
```




<hr>



### function sync [3/3]

```C++
void muda::ComputeGraphVarManager::sync (
    const span< const ComputeGraphVarBase * > vars
) const
```




<hr>



### function sync\_on [1/3]

```C++
void muda::ComputeGraphVarManager::sync_on (
    cudaStream_t stream
) const
```




<hr>



### function sync\_on [2/3]

```C++
template<typename... T>
void muda::ComputeGraphVarManager::sync_on (
    cudaStream_t stream,
    const ComputeGraphVar < T > &... vars
) const
```




<hr>



### function sync\_on [3/3]

```C++
void muda::ComputeGraphVarManager::sync_on (
    cudaStream_t stream,
    const span< const ComputeGraphVarBase * > vars
) const
```




<hr>



### function ~ComputeGraphVarManager 

```C++
muda::ComputeGraphVarManager::~ComputeGraphVarManager () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/compute_graph/compute_graph_var_manager.h`

