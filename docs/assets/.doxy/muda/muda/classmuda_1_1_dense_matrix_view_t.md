

# Class muda::DenseMatrixViewT

**template &lt;bool IsConst, typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseMatrixViewT**](classmuda_1_1_dense_matrix_view_t.md)








Inherits the following classes: [muda::ViewBase](classmuda_1_1_view_base.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef Buffer2DView&lt; Ty &gt; | [**Buffer2DView**](#typedef-buffer2dview)  <br> |
| typedef CBuffer2DView&lt; Ty &gt; | [**CBuffer2DView**](#typedef-cbuffer2dview)  <br> |
| typedef [**CDenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; Ty &gt; | [**CViewer**](#typedef-cviewer)  <br> |
| typedef [**DenseMatrixViewT**](classmuda_1_1_dense_matrix_view_t.md)&lt; true, Ty &gt; | [**ConstView**](#typedef-constview)  <br> |
| typedef [**DenseMatrixViewT**](classmuda_1_1_dense_matrix_view_t.md)&lt; false, Ty &gt; | [**NonConstView**](#typedef-nonconstview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBuffer2DView, Buffer2DView &gt; | [**ThisBuffer2DView**](#typedef-thisbuffer2dview)  <br> |
| typedef [**DenseMatrixViewT**](classmuda_1_1_dense_matrix_view_t.md)&lt; IsConst, Ty &gt; | [**ThisView**](#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_dense_matrix_viewer_t.md), [**Viewer**](classmuda_1_1_dense_matrix_viewer_t.md) &gt; | [**ThisViewer**](#typedef-thisviewer)  <br> |
| typedef [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer_t.md)&lt; Ty &gt; | [**Viewer**](#typedef-viewer)  <br> |


## Public Types inherited from muda::ViewBase

See [muda::ViewBase](classmuda_1_1_view_base.md)

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const T, T &gt; | [**auto\_const\_t**](classmuda_1_1_view_base.md#typedef-auto_const_t)  <br> |
| typedef std::enable\_if\_t&lt; IsNonConst, T &gt; | [**non\_const\_enable\_t**](classmuda_1_1_view_base.md#typedef-non_const_enable_t)  <br> |












## Public Static Attributes inherited from muda::ViewBase

See [muda::ViewBase](classmuda_1_1_view_base.md)

| Type | Name |
| ---: | :--- |
|  bool | [**IsConst**](classmuda_1_1_view_base.md#variable-isconst)   = = IsConst\_<br> |
|  bool | [**IsNonConst**](classmuda_1_1_view_base.md#variable-isnonconst)   = = !IsConst\_<br> |


























## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseMatrixViewT**](#function-densematrixviewt-23) (ThisBuffer2DView view, size\_t row, size\_t col, bool trans=false, bool sym=false) <br> |
|  MUDA\_GENERIC | [**DenseMatrixViewT**](#function-densematrixviewt-33) (const [**DenseMatrixViewT**](classmuda_1_1_dense_matrix_view_t.md)&lt; OtherIsConst, Ty &gt; & other) <br> |
|  MUDA\_GENERIC auto | [**T**](#function-t) () <br> |
|  MUDA\_GENERIC auto | [**as\_const**](#function-as_const) () const<br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](#function-buffer_view) () const<br> |
|  MUDA\_GENERIC size\_t | [**col**](#function-col) () const<br> |
|  MUDA\_GENERIC auto | [**cviewer**](#function-cviewer) () <br> |
|  MUDA\_GENERIC auto | [**data**](#function-data) () const<br> |
|  MUDA\_GENERIC bool | [**is\_sym**](#function-is_sym) () const<br> |
|  MUDA\_GENERIC bool | [**is\_trans**](#function-is_trans) () const<br> |
|  MUDA\_GENERIC size\_t | [**lda**](#function-lda) () const<br> |
|  MUDA\_GENERIC size\_t | [**row**](#function-row) () const<br> |
|  MUDA\_GENERIC auto | [**viewer**](#function-viewer) () <br> |
















## Protected Attributes

| Type | Name |
| ---: | :--- |
|  size\_t | [**m\_col**](#variable-m_col)   = = 0<br> |
|  size\_t | [**m\_row**](#variable-m_row)   = = 0<br> |
|  bool | [**m\_sym**](#variable-m_sym)   = = false<br> |
|  bool | [**m\_trans**](#variable-m_trans)   = = false<br> |
|  ThisBuffer2DView | [**m\_view**](#variable-m_view)  <br> |








































## Public Types Documentation




### typedef Buffer2DView 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::Buffer2DView =  Buffer2DView<Ty>;
```




<hr>



### typedef CBuffer2DView 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::CBuffer2DView =  CBuffer2DView<Ty>;
```




<hr>



### typedef CViewer 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::CViewer =  CDenseMatrixViewer<Ty>;
```




<hr>



### typedef ConstView 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::ConstView =  DenseMatrixViewT<true, Ty>;
```




<hr>



### typedef NonConstView 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::NonConstView =  DenseMatrixViewT<false, Ty>;
```




<hr>



### typedef ThisBuffer2DView 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::ThisBuffer2DView =  std::conditional_t<IsConst, CBuffer2DView, Buffer2DView>;
```




<hr>



### typedef ThisView 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::ThisView =  DenseMatrixViewT<IsConst, Ty>;
```




<hr>



### typedef ThisViewer 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::ThisViewer =  std::conditional_t<IsConst, CViewer, Viewer>;
```




<hr>



### typedef Viewer 

```C++
using muda::DenseMatrixViewT< IsConst, Ty >::Viewer =  DenseMatrixViewer<Ty>;
```




<hr>
## Public Functions Documentation




### function DenseMatrixViewT [2/3]

```C++
inline MUDA_GENERIC muda::DenseMatrixViewT::DenseMatrixViewT (
    ThisBuffer2DView view,
    size_t row,
    size_t col,
    bool trans=false,
    bool sym=false
) 
```




<hr>



### function DenseMatrixViewT [3/3]

```C++
template<bool OtherIsConst>
inline MUDA_GENERIC muda::DenseMatrixViewT::DenseMatrixViewT (
    const DenseMatrixViewT < OtherIsConst, Ty > & other
) 
```




<hr>



### function T 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewT::T () 
```




<hr>



### function as\_const 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewT::as_const () const
```




<hr>



### function buffer\_view 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewT::buffer_view () const
```




<hr>



### function col 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewT::col () const
```




<hr>



### function cviewer 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewT::cviewer () 
```




<hr>



### function data 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewT::data () const
```




<hr>



### function is\_sym 

```C++
inline MUDA_GENERIC bool muda::DenseMatrixViewT::is_sym () const
```




<hr>



### function is\_trans 

```C++
inline MUDA_GENERIC bool muda::DenseMatrixViewT::is_trans () const
```




<hr>



### function lda 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewT::lda () const
```




<hr>



### function row 

```C++
inline MUDA_GENERIC size_t muda::DenseMatrixViewT::row () const
```




<hr>



### function viewer 

```C++
inline MUDA_GENERIC auto muda::DenseMatrixViewT::viewer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_col 

```C++
size_t muda::DenseMatrixViewT< IsConst, Ty >::m_col;
```




<hr>



### variable m\_row 

```C++
size_t muda::DenseMatrixViewT< IsConst, Ty >::m_row;
```




<hr>



### variable m\_sym 

```C++
bool muda::DenseMatrixViewT< IsConst, Ty >::m_sym;
```




<hr>



### variable m\_trans 

```C++
bool muda::DenseMatrixViewT< IsConst, Ty >::m_trans;
```




<hr>



### variable m\_view 

```C++
ThisBuffer2DView muda::DenseMatrixViewT< IsConst, Ty >::m_view;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_matrix_view.h`

