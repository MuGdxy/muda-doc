

# Class muda::DenseMatrixView

**template &lt;typename Ty&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**DenseMatrixView**](classmuda_1_1_dense_matrix_view.md)








Inherits the following classes: [muda::DenseMatrixViewBase](classmuda_1_1_dense_matrix_view_base.md)
















## Public Types inherited from muda::DenseMatrixViewBase

See [muda::DenseMatrixViewBase](classmuda_1_1_dense_matrix_view_base.md)

| Type | Name |
| ---: | :--- |
| typedef Buffer2DView&lt; Ty &gt; | [**Buffer2DView**](classmuda_1_1_dense_matrix_view_base.md#typedef-buffer2dview)  <br> |
| typedef CBuffer2DView&lt; Ty &gt; | [**CBuffer2DView**](classmuda_1_1_dense_matrix_view_base.md#typedef-cbuffer2dview)  <br> |
| typedef [**CDenseMatrixViewer**](classmuda_1_1_c_dense_matrix_viewer.md)&lt; Ty &gt; | [**CViewer**](classmuda_1_1_dense_matrix_view_base.md#typedef-cviewer)  <br> |
| typedef [**DenseMatrixViewBase**](classmuda_1_1_dense_matrix_view_base.md)&lt; true, Ty &gt; | [**ConstView**](classmuda_1_1_dense_matrix_view_base.md#typedef-constview)  <br> |
| typedef [**DenseMatrixViewBase**](classmuda_1_1_dense_matrix_view_base.md)&lt; false, Ty &gt; | [**NonConstView**](classmuda_1_1_dense_matrix_view_base.md#typedef-nonconstview)  <br> |
| typedef std::conditional\_t&lt; IsConst, CBuffer2DView, Buffer2DView &gt; | [**ThisBuffer2DView**](classmuda_1_1_dense_matrix_view_base.md#typedef-thisbuffer2dview)  <br> |
| typedef [**DenseMatrixViewBase**](classmuda_1_1_dense_matrix_view_base.md)&lt; IsConst, Ty &gt; | [**ThisView**](classmuda_1_1_dense_matrix_view_base.md#typedef-thisview)  <br> |
| typedef std::conditional\_t&lt; IsConst, [**CViewer**](classmuda_1_1_c_dense_matrix_viewer.md), [**Viewer**](classmuda_1_1_dense_matrix_viewer.md) &gt; | [**ThisViewer**](classmuda_1_1_dense_matrix_view_base.md#typedef-thisviewer)  <br> |
| typedef [**DenseMatrixViewer**](classmuda_1_1_dense_matrix_viewer.md)&lt; Ty &gt; | [**Viewer**](classmuda_1_1_dense_matrix_view_base.md#typedef-viewer)  <br> |


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
|  constexpr bool | [**IsConst**](classmuda_1_1_view_base.md#variable-isconst)   = = IsConst\_<br> |
|  constexpr bool | [**IsNonConst**](classmuda_1_1_view_base.md#variable-isnonconst)   = = !IsConst\_<br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DenseMatrixView**](#function-densematrixview-12) (const [**Base**](classmuda_1_1_dense_matrix_view_base.md) & base) <br> |
|   | [**DenseMatrixView**](#function-densematrixview-22) (const [**CDenseMatrixView**](classmuda_1_1_c_dense_matrix_view.md)&lt; Ty &gt; &) = delete<br> |
|  auto | [**T**](#function-t) () const<br> |


## Public Functions inherited from muda::DenseMatrixViewBase

See [muda::DenseMatrixViewBase](classmuda_1_1_dense_matrix_view_base.md)

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**DenseMatrixViewBase**](classmuda_1_1_dense_matrix_view_base.md#function-densematrixviewbase) (ThisBuffer2DView view, size\_t row, size\_t col, bool trans=false, bool sym=false) <br> |
|  MUDA\_GENERIC [**ThisView**](classmuda_1_1_dense_matrix_view_base.md) | [**T**](classmuda_1_1_dense_matrix_view_base.md#function-t-12) () <br> |
|  MUDA\_GENERIC [**ConstView**](classmuda_1_1_dense_matrix_view_base.md) | [**T**](classmuda_1_1_dense_matrix_view_base.md#function-t-22) () const<br> |
|  MUDA\_GENERIC auto | [**as\_const**](classmuda_1_1_dense_matrix_view_base.md#function-as_const) () const<br> |
|  MUDA\_GENERIC auto | [**buffer\_view**](classmuda_1_1_dense_matrix_view_base.md#function-buffer_view-12) () <br> |
|  MUDA\_GENERIC CBuffer2DView | [**buffer\_view**](classmuda_1_1_dense_matrix_view_base.md#function-buffer_view-22) () const<br> |
|  MUDA\_GENERIC size\_t | [**col**](classmuda_1_1_dense_matrix_view_base.md#function-col) () const<br> |
|  MUDA\_GENERIC [**CViewer**](classmuda_1_1_c_dense_matrix_viewer.md) | [**cviewer**](classmuda_1_1_dense_matrix_view_base.md#function-cviewer) () const<br> |
|  MUDA\_GENERIC auto | [**data**](classmuda_1_1_dense_matrix_view_base.md#function-data-12) () <br> |
|  MUDA\_GENERIC auto | [**data**](classmuda_1_1_dense_matrix_view_base.md#function-data-22) () const<br> |
|  MUDA\_GENERIC bool | [**is\_sym**](classmuda_1_1_dense_matrix_view_base.md#function-is_sym) () const<br> |
|  MUDA\_GENERIC bool | [**is\_trans**](classmuda_1_1_dense_matrix_view_base.md#function-is_trans) () const<br> |
|  MUDA\_GENERIC size\_t | [**lda**](classmuda_1_1_dense_matrix_view_base.md#function-lda) () const<br> |
|  MUDA\_GENERIC | [**operator ConstView**](classmuda_1_1_dense_matrix_view_base.md#function-operator-constview) () const<br> |
|  MUDA\_GENERIC size\_t | [**row**](classmuda_1_1_dense_matrix_view_base.md#function-row) () const<br> |
|  MUDA\_GENERIC ThisViewer | [**viewer**](classmuda_1_1_dense_matrix_view_base.md#function-viewer) () <br> |
























## Protected Attributes inherited from muda::DenseMatrixViewBase

See [muda::DenseMatrixViewBase](classmuda_1_1_dense_matrix_view_base.md)

| Type | Name |
| ---: | :--- |
|  size\_t | [**m\_col**](classmuda_1_1_dense_matrix_view_base.md#variable-m_col)   = = 0<br> |
|  size\_t | [**m\_row**](classmuda_1_1_dense_matrix_view_base.md#variable-m_row)   = = 0<br> |
|  bool | [**m\_sym**](classmuda_1_1_dense_matrix_view_base.md#variable-m_sym)   = = false<br> |
|  bool | [**m\_trans**](classmuda_1_1_dense_matrix_view_base.md#variable-m_trans)   = = false<br> |
|  ThisBuffer2DView | [**m\_view**](classmuda_1_1_dense_matrix_view_base.md#variable-m_view)  <br> |


























































## Public Functions Documentation




### function DenseMatrixView [1/2]

```C++
inline muda::DenseMatrixView::DenseMatrixView (
    const Base & base
) 
```




<hr>



### function DenseMatrixView [2/2]

```C++
muda::DenseMatrixView::DenseMatrixView (
    const CDenseMatrixView < Ty > &
) = delete
```




<hr>



### function T 

```C++
inline auto muda::DenseMatrixView::T () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/dense_matrix_view.h`

