

# Class muda::GraphViewer



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**GraphViewer**](classmuda_1_1_graph_viewer.md)








Inherits the following classes: [muda::ViewerBase](classmuda_1_1_viewer_base.md)




























## Public Static Attributes inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_viewer_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_viewer_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**GraphViewer**](#function-graphviewer-12) () = default<br> |
|  MUDA\_GENERIC | [**GraphViewer**](#function-graphviewer-22) (cudaGraphExec\_t graph, [**Flags**](classmuda_1_1_flags.md)&lt; GraphInstantiateFlagBit &gt; flags) <br> |
|  MUDA\_DEVICE void | [**fire\_and\_forget**](#function-fire_and_forget) () const<br> |
|  MUDA\_GENERIC auto | [**handle**](#function-handle) () const<br> |
|  MUDA\_GENERIC void | [**launch**](#function-launch) (cudaStream\_t stream=nullptr) const<br> |
|  MUDA\_DEVICE void | [**tail\_launch**](#function-tail_launch) () const<br> |


## Public Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-13) () <br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-23) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|   | [**ViewerBase**](classmuda_1_1_viewer_base.md#function-viewerbase-33) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**copy\_label**](classmuda_1_1_viewer_base.md#function-copy_label) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) & other) <br> |
|  MUDA\_GENERIC const char \* | [**kernel\_file**](classmuda_1_1_viewer_base.md#function-kernel_file) () const<br> |
|  MUDA\_GENERIC int | [**kernel\_line**](classmuda_1_1_viewer_base.md#function-kernel_line) () const<br> |
|  MUDA\_GENERIC const char \* | [**kernel\_name**](classmuda_1_1_viewer_base.md#function-kernel_name) () const<br> |
|  MUDA\_GENERIC const char \* | [**name**](classmuda_1_1_viewer_base.md#function-name-13) () const<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator) (const [**ViewerBase**](classmuda_1_1_viewer_base.md) &) = default<br> |
|  [**ViewerBase**](classmuda_1_1_viewer_base.md) & | [**operator=**](classmuda_1_1_viewer_base.md#function-operator_1) ([**ViewerBase**](classmuda_1_1_viewer_base.md) &&) = default<br> |








## Protected Types inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_viewer_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_viewer_base.md#typedef-non_const_enable_t)  <br> |








































## Protected Functions inherited from muda::ViewerBase

See [muda::ViewerBase](classmuda_1_1_viewer_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_INLINE MUDA\_HOST void | [**name**](classmuda_1_1_viewer_base.md#function-name-23) (const char \* n) <br> |
|  MUDA\_INLINE MUDA\_GENERIC void | [**name**](classmuda_1_1_viewer_base.md#function-name-33) ([**details::StringPointer**](classmuda_1_1details_1_1_string_pointer.md) pointer) <br> |






## Public Functions Documentation




### function GraphViewer [1/2]

```C++
MUDA_GENERIC muda::GraphViewer::GraphViewer () = default
```




<hr>



### function GraphViewer [2/2]

```C++
MUDA_GENERIC muda::GraphViewer::GraphViewer (
    cudaGraphExec_t graph,
    Flags < GraphInstantiateFlagBit > flags
) 
```




<hr>



### function fire\_and\_forget 

```C++
MUDA_DEVICE void muda::GraphViewer::fire_and_forget () const
```




<hr>



### function handle 

```C++
inline MUDA_GENERIC auto muda::GraphViewer::handle () const
```




<hr>



### function launch 

```C++
MUDA_GENERIC void muda::GraphViewer::launch (
    cudaStream_t stream=nullptr
) const
```




<hr>



### function tail\_launch 

```C++
MUDA_DEVICE void muda::GraphViewer::tail_launch () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/graph/graph_viewer.h`

