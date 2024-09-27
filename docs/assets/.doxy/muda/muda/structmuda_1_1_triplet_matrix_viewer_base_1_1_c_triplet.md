

# Struct muda::TripletMatrixViewerBase::CTriplet



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**TripletMatrixViewerBase**](classmuda_1_1_triplet_matrix_viewer_base.md) **>** [**CTriplet**](structmuda_1_1_triplet_matrix_viewer_base_1_1_c_triplet.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  int | [**block\_col\_index**](#variable-block_col_index)  <br> |
|  int | [**block\_row\_index**](#variable-block_row_index)  <br> |
|  const BlockMatrix & | [**block\_value**](#variable-block_value)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC | [**CTriplet**](#function-ctriplet) (int row\_index, int col\_index, const BlockMatrix & block) <br> |




























## Public Attributes Documentation




### variable block\_col\_index 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, N >::CTriplet::block_col_index;
```




<hr>



### variable block\_row\_index 

```C++
int muda::TripletMatrixViewerBase< IsConst, T, N >::CTriplet::block_row_index;
```




<hr>



### variable block\_value 

```C++
const BlockMatrix& muda::TripletMatrixViewerBase< IsConst, T, N >::CTriplet::block_value;
```




<hr>
## Public Functions Documentation




### function CTriplet 

```C++
inline MUDA_GENERIC muda::TripletMatrixViewerBase::CTriplet::CTriplet (
    int row_index,
    int col_index,
    const BlockMatrix & block
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/linear_system/triplet_matrix_viewer.h`

