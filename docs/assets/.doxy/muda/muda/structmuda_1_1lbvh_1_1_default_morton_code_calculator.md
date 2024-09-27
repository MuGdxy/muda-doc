

# Struct muda::lbvh::DefaultMortonCodeCalculator

**template &lt;typename Real, typename Object&gt;**



[**ClassList**](annotated.md) **>** [**muda**](namespacemuda.md) **>** [**lbvh**](namespacemuda_1_1lbvh.md) **>** [**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; | [**whole**](#variable-whole)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DefaultMortonCodeCalculator**](#function-defaultmortoncodecalculator-14) ([**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; w) <br> |
|   | [**DefaultMortonCodeCalculator**](#function-defaultmortoncodecalculator-24) () = default<br> |
|   | [**DefaultMortonCodeCalculator**](#function-defaultmortoncodecalculator-34) ([**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) const &) = default<br> |
|   | [**DefaultMortonCodeCalculator**](#function-defaultmortoncodecalculator-44) ([**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) &&) = default<br> |
|  \_\_device\_\_ \_\_host\_\_ uint32\_t | [**operator()**](#function-operator()) (const Object &, const [**AABB**](structmuda_1_1lbvh_1_1_a_a_b_b.md)&lt; Real &gt; & box) noexcept<br> |
|  [**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) & | [**operator=**](#function-operator) ([**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) const &) = default<br> |
|  [**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) & | [**operator=**](#function-operator_1) ([**DefaultMortonCodeCalculator**](structmuda_1_1lbvh_1_1_default_morton_code_calculator.md) &&) = default<br> |
|   | [**~DefaultMortonCodeCalculator**](#function-defaultmortoncodecalculator) () = default<br> |




























## Public Attributes Documentation




### variable whole 

```C++
AABB<Real> muda::lbvh::DefaultMortonCodeCalculator< Real, Object >::whole;
```




<hr>
## Public Functions Documentation




### function DefaultMortonCodeCalculator [1/4]

```C++
inline muda::lbvh::DefaultMortonCodeCalculator::DefaultMortonCodeCalculator (
    AABB < Real > w
) 
```




<hr>



### function DefaultMortonCodeCalculator [2/4]

```C++
muda::lbvh::DefaultMortonCodeCalculator::DefaultMortonCodeCalculator () = default
```




<hr>



### function DefaultMortonCodeCalculator [3/4]

```C++
muda::lbvh::DefaultMortonCodeCalculator::DefaultMortonCodeCalculator (
    DefaultMortonCodeCalculator const &
) = default
```




<hr>



### function DefaultMortonCodeCalculator [4/4]

```C++
muda::lbvh::DefaultMortonCodeCalculator::DefaultMortonCodeCalculator (
    DefaultMortonCodeCalculator &&
) = default
```




<hr>



### function operator() 

```C++
inline __device__ __host__ uint32_t muda::lbvh::DefaultMortonCodeCalculator::operator() (
    const Object &,
    const AABB < Real > & box
) noexcept
```




<hr>



### function operator= 

```C++
DefaultMortonCodeCalculator & muda::lbvh::DefaultMortonCodeCalculator::operator= (
    DefaultMortonCodeCalculator const &
) = default
```




<hr>



### function operator= 

```C++
DefaultMortonCodeCalculator & muda::lbvh::DefaultMortonCodeCalculator::operator= (
    DefaultMortonCodeCalculator &&
) = default
```




<hr>



### function ~DefaultMortonCodeCalculator 

```C++
muda::lbvh::DefaultMortonCodeCalculator::~DefaultMortonCodeCalculator () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/lbvh/bvh.h`

