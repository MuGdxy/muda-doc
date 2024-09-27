

# Namespace muda::distance



[**Namespace List**](namespaces.md) **>** [**muda**](namespacemuda.md) **>** [**distance**](namespacemuda_1_1distance.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum unsigned char | [**EdgeEdgeDistanceType**](#enum-edgeedgedistancetype)  <br> |
| enum unsigned char | [**PointEdgeDistanceType**](#enum-pointedgedistancetype)  <br> |
| enum unsigned char | [**PointPointDistanceType**](#enum-pointpointdistancetype)  <br> |
| enum unsigned char | [**PointTriangleDistanceType**](#enum-pointtriangledistancetype)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  MUDA\_GENERIC bool | [**edge\_edge\_ccd**](#function-edge_edge_ccd) (Eigen::Matrix&lt; T, 3, 1 &gt; ea0, Eigen::Matrix&lt; T, 3, 1 &gt; ea1, Eigen::Matrix&lt; T, 3, 1 &gt; eb0, Eigen::Matrix&lt; T, 3, 1 &gt; eb1, Eigen::Matrix&lt; T, 3, 1 &gt; dea0, Eigen::Matrix&lt; T, 3, 1 &gt; dea1, Eigen::Matrix&lt; T, 3, 1 &gt; deb0, Eigen::Matrix&lt; T, 3, 1 &gt; deb1, T eta, T thickness, int max\_iter, T & toc) <br> |
|  MUDA\_GENERIC bool | [**edge\_edge\_ccd\_broadphase**](#function-edge_edge_ccd_broadphase) (const Eigen::Matrix&lt; T, 3, 1 &gt; & ea0, const Eigen::Matrix&lt; T, 3, 1 &gt; & ea1, const Eigen::Matrix&lt; T, 3, 1 &gt; & eb0, const Eigen::Matrix&lt; T, 3, 1 &gt; & eb1, const Eigen::Matrix&lt; T, 3, 1 &gt; & dea0, const Eigen::Matrix&lt; T, 3, 1 &gt; & dea1, const Eigen::Matrix&lt; T, 3, 1 &gt; & deb0, const Eigen::Matrix&lt; T, 3, 1 &gt; & deb1, T dist) <br> |
|  MUDA\_GENERIC bool | [**edge\_edge\_cd\_broadphase**](#function-edge_edge_cd_broadphase) (const Eigen::Matrix&lt; T, 3, 1 &gt; & ea0, const Eigen::Matrix&lt; T, 3, 1 &gt; & ea1, const Eigen::Matrix&lt; T, 3, 1 &gt; & eb0, const Eigen::Matrix&lt; T, 3, 1 &gt; & eb1, T dist) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_cross\_norm2**](#function-edge_edge_cross_norm2) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, T & result) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_cross\_norm2\_gradient**](#function-edge_edge_cross_norm2_gradient) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, Eigen::Vector&lt; T, 12 &gt; & grad) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_cross\_norm2\_hessian**](#function-edge_edge_cross_norm2_hessian) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, Eigen::Matrix&lt; T, 12, 12 &gt; & Hessian) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_distance**](#function-edge_edge_distance) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, T & dist2) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_distance\_gradient**](#function-edge_edge_distance_gradient) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, Eigen::Vector&lt; T, 12 &gt; & grad) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_distance\_hessian**](#function-edge_edge_distance_hessian) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, Eigen::Matrix&lt; T, 12, 12 &gt; & Hessian) <br> |
|  MUDA\_GENERIC EdgeEdgeDistanceType | [**edge\_edge\_distance\_type**](#function-edge_edge_distance_type) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_distance\_unclassified**](#function-edge_edge_distance_unclassified) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, T & dist2) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_mollifier**](#function-edge_edge_mollifier) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, T eps\_x, T & e) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_mollifier\_gradient**](#function-edge_edge_mollifier_gradient) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, T eps\_x, Eigen::Vector&lt; T, 12 &gt; & g) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_mollifier\_hessian**](#function-edge_edge_mollifier_hessian) (const Eigen::Vector&lt; T, 3 &gt; & ea0, const Eigen::Vector&lt; T, 3 &gt; & ea1, const Eigen::Vector&lt; T, 3 &gt; & eb0, const Eigen::Vector&lt; T, 3 &gt; & eb1, T eps\_x, Eigen::Matrix&lt; T, 12, 12 &gt; & H) <br> |
|  MUDA\_GENERIC void | [**edge\_edge\_mollifier\_threshold**](#function-edge_edge_mollifier_threshold) (const Eigen::Vector&lt; T, 3 &gt; & ea0\_rest, const Eigen::Vector&lt; T, 3 &gt; & ea1\_rest, const Eigen::Vector&lt; T, 3 &gt; & eb0\_rest, const Eigen::Vector&lt; T, 3 &gt; & eb1\_rest, T & eps\_x) <br> |
|  MUDA\_GENERIC bool | [**point\_edge\_ccd**](#function-point_edge_ccd) (const Eigen::Matrix&lt; T, 2, 1 &gt; & x0, const Eigen::Matrix&lt; T, 2, 1 &gt; & x1, const Eigen::Matrix&lt; T, 2, 1 &gt; & x2, const Eigen::Matrix&lt; T, 2, 1 &gt; & d0, const Eigen::Matrix&lt; T, 2, 1 &gt; & d1, const Eigen::Matrix&lt; T, 2, 1 &gt; & d2, T eta, T & toc) <br> |
|  MUDA\_GENERIC bool | [**point\_edge\_ccd**](#function-point_edge_ccd) (Eigen::Matrix&lt; T, 3, 1 &gt; p, Eigen::Matrix&lt; T, 3, 1 &gt; e0, Eigen::Matrix&lt; T, 3, 1 &gt; e1, Eigen::Matrix&lt; T, 3, 1 &gt; dp, Eigen::Matrix&lt; T, 3, 1 &gt; de0, Eigen::Matrix&lt; T, 3, 1 &gt; de1, T eta, T thickness, int max\_iter, T & toc) <br> |
|  MUDA\_GENERIC bool | [**point\_edge\_ccd\_broadphase**](#function-point_edge_ccd_broadphase) (const Eigen::Matrix&lt; T, 2, 1 &gt; & p, const Eigen::Matrix&lt; T, 2, 1 &gt; & e0, const Eigen::Matrix&lt; T, 2, 1 &gt; & e1, const Eigen::Matrix&lt; T, 2, 1 &gt; & dp, const Eigen::Matrix&lt; T, 2, 1 &gt; & de0, const Eigen::Matrix&lt; T, 2, 1 &gt; & de1, T dist) <br> |
|  MUDA\_GENERIC bool | [**point\_edge\_ccd\_broadphase**](#function-point_edge_ccd_broadphase) (const Eigen::Matrix&lt; T, 3, 1 &gt; & p, const Eigen::Matrix&lt; T, 3, 1 &gt; & e0, const Eigen::Matrix&lt; T, 3, 1 &gt; & e1, const Eigen::Matrix&lt; T, 3, 1 &gt; & dp, const Eigen::Matrix&lt; T, 3, 1 &gt; & de0, const Eigen::Matrix&lt; T, 3, 1 &gt; & de1, T dist) <br> |
|  MUDA\_GENERIC bool | [**point\_edge\_cd\_broadphase**](#function-point_edge_cd_broadphase) (const Eigen::Matrix&lt; T, dim, 1 &gt; & x0, const Eigen::Matrix&lt; T, dim, 1 &gt; & x1, const Eigen::Matrix&lt; T, dim, 1 &gt; & x2, T dist) <br> |
|  MUDA\_GENERIC void | [**point\_edge\_distance**](#function-point_edge_distance) (const Eigen::Vector&lt; T, dim &gt; & p, const Eigen::Vector&lt; T, dim &gt; & e0, const Eigen::Vector&lt; T, dim &gt; & e1, T & dist2) <br> |
|  MUDA\_GENERIC void | [**point\_edge\_distance\_gradient**](#function-point_edge_distance_gradient) (const Eigen::Vector&lt; T, dim &gt; & p, const Eigen::Vector&lt; T, dim &gt; & e0, const Eigen::Vector&lt; T, dim &gt; & e1, Eigen::Vector&lt; T, dim \*3 &gt; & grad) <br> |
|  MUDA\_GENERIC void | [**point\_edge\_distance\_hessian**](#function-point_edge_distance_hessian) (const Eigen::Vector&lt; T, dim &gt; & p, const Eigen::Vector&lt; T, dim &gt; & e0, const Eigen::Vector&lt; T, dim &gt; & e1, Eigen::Matrix&lt; T, dim \*3, dim \*3 &gt; & Hessian) <br> |
|  MUDA\_GENERIC PointEdgeDistanceType | [**point\_edge\_distance\_type**](#function-point_edge_distance_type) (const Eigen::Vector&lt; T, dim &gt; & p, const Eigen::Vector&lt; T, dim &gt; & e0, const Eigen::Vector&lt; T, dim &gt; & e1) <br> |
|  MUDA\_GENERIC PointEdgeDistanceType | [**point\_edge\_distance\_type**](#function-point_edge_distance_type) (const Eigen::Vector&lt; T, dim &gt; & p, const Eigen::Vector&lt; T, dim &gt; & e0, const Eigen::Vector&lt; T, dim &gt; & e1, T & ratio) <br> |
|  MUDA\_GENERIC void | [**point\_edge\_distance\_unclassified**](#function-point_edge_distance_unclassified) (const Eigen::Vector&lt; T, 3 &gt; & p, const Eigen::Vector&lt; T, 3 &gt; & e0, const Eigen::Vector&lt; T, 3 &gt; & e1, T & dist2) <br> |
|  MUDA\_GENERIC bool | [**point\_point\_ccd**](#function-point_point_ccd) (Eigen::Matrix&lt; T, 3, 1 &gt; p0, Eigen::Matrix&lt; T, 3, 1 &gt; p1, Eigen::Matrix&lt; T, 3, 1 &gt; dp0, Eigen::Matrix&lt; T, 3, 1 &gt; dp1, T eta, T thickness, int max\_iter, T & toc) <br> |
|  MUDA\_GENERIC bool | [**point\_point\_ccd\_broadphase**](#function-point_point_ccd_broadphase) (const Eigen::Matrix&lt; T, 3, 1 &gt; & p0, const Eigen::Matrix&lt; T, 3, 1 &gt; & p1, const Eigen::Matrix&lt; T, 3, 1 &gt; & dp0, const Eigen::Matrix&lt; T, 3, 1 &gt; & dp1, T dist) <br> |
|  MUDA\_GENERIC void | [**point\_point\_distance**](#function-point_point_distance) (const Eigen::Vector&lt; T, dim &gt; & a, const Eigen::Vector&lt; T, dim &gt; & b, T & dist2) <br> |
|  MUDA\_GENERIC void | [**point\_point\_distance\_gradient**](#function-point_point_distance_gradient) (const Eigen::Vector&lt; T, dim &gt; & a, const Eigen::Vector&lt; T, dim &gt; & b, Eigen::Vector&lt; T, dim \*2 &gt; & grad) <br> |
|  MUDA\_GENERIC void | [**point\_point\_distance\_hessian**](#function-point_point_distance_hessian) (const Eigen::Vector&lt; T, dim &gt; & a, const Eigen::Vector&lt; T, dim &gt; & b, Eigen::Matrix&lt; T, dim \*2, dim \*2 &gt; & Hessian) <br> |
|  MUDA\_GENERIC PointPointDistanceType | [**point\_point\_distance\_type**](#function-point_point_distance_type) (const Eigen::Vector&lt; T, dim &gt; & p0, const Eigen::Vector&lt; T, dim &gt; & p1) <br> |
|  MUDA\_GENERIC void | [**point\_point\_distance\_unclassified**](#function-point_point_distance_unclassified) (const Eigen::Vector&lt; T, 3 &gt; & p0, const Eigen::Vector&lt; T, 3 &gt; & p1, T & dist2) <br> |
|  MUDA\_GENERIC bool | [**point\_triangle\_ccd**](#function-point_triangle_ccd) (Eigen::Matrix&lt; T, 3, 1 &gt; p, Eigen::Matrix&lt; T, 3, 1 &gt; t0, Eigen::Matrix&lt; T, 3, 1 &gt; t1, Eigen::Matrix&lt; T, 3, 1 &gt; t2, Eigen::Matrix&lt; T, 3, 1 &gt; dp, Eigen::Matrix&lt; T, 3, 1 &gt; dt0, Eigen::Matrix&lt; T, 3, 1 &gt; dt1, Eigen::Matrix&lt; T, 3, 1 &gt; dt2, T eta, T thickness, int max\_iter, T & toc) <br> |
|  MUDA\_GENERIC bool | [**point\_triangle\_ccd\_broadphase**](#function-point_triangle_ccd_broadphase) (const Eigen::Matrix&lt; T, 3, 1 &gt; & p, const Eigen::Matrix&lt; T, 3, 1 &gt; & t0, const Eigen::Matrix&lt; T, 3, 1 &gt; & t1, const Eigen::Matrix&lt; T, 3, 1 &gt; & t2, const Eigen::Matrix&lt; T, 3, 1 &gt; & dp, const Eigen::Matrix&lt; T, 3, 1 &gt; & dt0, const Eigen::Matrix&lt; T, 3, 1 &gt; & dt1, const Eigen::Matrix&lt; T, 3, 1 &gt; & dt2, T dist) <br> |
|  MUDA\_GENERIC bool | [**point\_triangle\_cd\_broadphase**](#function-point_triangle_cd_broadphase) (const Eigen::Matrix&lt; T, 3, 1 &gt; & p, const Eigen::Matrix&lt; T, 3, 1 &gt; & t0, const Eigen::Matrix&lt; T, 3, 1 &gt; & t1, const Eigen::Matrix&lt; T, 3, 1 &gt; & t2, T dist) <br> |
|  MUDA\_GENERIC void | [**point\_triangle\_distance**](#function-point_triangle_distance) (const Eigen::Vector&lt; T, 3 &gt; & p, const Eigen::Vector&lt; T, 3 &gt; & t0, const Eigen::Vector&lt; T, 3 &gt; & t1, const Eigen::Vector&lt; T, 3 &gt; & t2, T & dist2) <br> |
|  MUDA\_GENERIC void | [**point\_triangle\_distance\_gradient**](#function-point_triangle_distance_gradient) (const Eigen::Vector&lt; T, 3 &gt; & p, const Eigen::Vector&lt; T, 3 &gt; & t0, const Eigen::Vector&lt; T, 3 &gt; & t1, const Eigen::Vector&lt; T, 3 &gt; & t2, Eigen::Vector&lt; T, 12 &gt; & grad) <br> |
|  MUDA\_GENERIC void | [**point\_triangle\_distance\_hessian**](#function-point_triangle_distance_hessian) (const Eigen::Vector&lt; T, 3 &gt; & p, const Eigen::Vector&lt; T, 3 &gt; & t0, const Eigen::Vector&lt; T, 3 &gt; & t1, const Eigen::Vector&lt; T, 3 &gt; & t2, Eigen::Matrix&lt; T, 12, 12 &gt; & Hessian) <br> |
|  MUDA\_GENERIC PointTriangleDistanceType | [**point\_triangle\_distance\_type**](#function-point_triangle_distance_type) (const Eigen::Vector&lt; T, 3 &gt; & p, const Eigen::Vector&lt; T, 3 &gt; & t0, const Eigen::Vector&lt; T, 3 &gt; & t1, const Eigen::Vector&lt; T, 3 &gt; & t2) <br> |
|  MUDA\_GENERIC void | [**point\_triangle\_distance\_unclassified**](#function-point_triangle_distance_unclassified) (const Eigen::Vector&lt; T, 3 &gt; & p, const Eigen::Vector&lt; T, 3 &gt; & t0, const Eigen::Vector&lt; T, 3 &gt; & t1, const Eigen::Vector&lt; T, 3 &gt; & t2, T & dist2) <br> |




























## Public Types Documentation




### enum EdgeEdgeDistanceType 

```C++
enum muda::distance::EdgeEdgeDistanceType {
    PP_Ea0Eb0 = 0,
    PP_Ea0Eb1 = 1,
    PE_Ea0Eb0Eb1 = 2,
    PP_Ea1Eb0 = 3,
    PP_Ea1Eb1 = 4,
    PE_Ea1Eb0Eb1 = 5,
    PE_Eb0Ea0Ea1 = 6,
    PE_Eb1Ea0Ea1 = 7,
    EE = 8
};
```




<hr>



### enum PointEdgeDistanceType 

```C++
enum muda::distance::PointEdgeDistanceType {
    PP_PE0 = 0,
    PP_PE1 = 1,
    PE = 2
};
```




<hr>



### enum PointPointDistanceType 

```C++
enum muda::distance::PointPointDistanceType {
    PP = 0
};
```




<hr>



### enum PointTriangleDistanceType 

```C++
enum muda::distance::PointTriangleDistanceType {
    PP_PT0 = 0,
    PP_PT1 = 1,
    PP_PT2 = 2,
    PE_PT0T1 = 3,
    PE_PT1T2 = 4,
    PE_PT2T0 = 5,
    PT = 6
};
```




<hr>
## Public Functions Documentation




### function edge\_edge\_ccd 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::edge_edge_ccd (
    Eigen::Matrix< T, 3, 1 > ea0,
    Eigen::Matrix< T, 3, 1 > ea1,
    Eigen::Matrix< T, 3, 1 > eb0,
    Eigen::Matrix< T, 3, 1 > eb1,
    Eigen::Matrix< T, 3, 1 > dea0,
    Eigen::Matrix< T, 3, 1 > dea1,
    Eigen::Matrix< T, 3, 1 > deb0,
    Eigen::Matrix< T, 3, 1 > deb1,
    T eta,
    T thickness,
    int max_iter,
    T & toc
) 
```




<hr>



### function edge\_edge\_ccd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::edge_edge_ccd_broadphase (
    const Eigen::Matrix< T, 3, 1 > & ea0,
    const Eigen::Matrix< T, 3, 1 > & ea1,
    const Eigen::Matrix< T, 3, 1 > & eb0,
    const Eigen::Matrix< T, 3, 1 > & eb1,
    const Eigen::Matrix< T, 3, 1 > & dea0,
    const Eigen::Matrix< T, 3, 1 > & dea1,
    const Eigen::Matrix< T, 3, 1 > & deb0,
    const Eigen::Matrix< T, 3, 1 > & deb1,
    T dist
) 
```




<hr>



### function edge\_edge\_cd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::edge_edge_cd_broadphase (
    const Eigen::Matrix< T, 3, 1 > & ea0,
    const Eigen::Matrix< T, 3, 1 > & ea1,
    const Eigen::Matrix< T, 3, 1 > & eb0,
    const Eigen::Matrix< T, 3, 1 > & eb1,
    T dist
) 
```




<hr>



### function edge\_edge\_cross\_norm2 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_cross_norm2 (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    T & result
) 
```




<hr>



### function edge\_edge\_cross\_norm2\_gradient 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_cross_norm2_gradient (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    Eigen::Vector< T, 12 > & grad
) 
```




<hr>



### function edge\_edge\_cross\_norm2\_hessian 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_cross_norm2_hessian (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    Eigen::Matrix< T, 12, 12 > & Hessian
) 
```




<hr>



### function edge\_edge\_distance 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_distance (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    T & dist2
) 
```




<hr>



### function edge\_edge\_distance\_gradient 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_distance_gradient (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    Eigen::Vector< T, 12 > & grad
) 
```




<hr>



### function edge\_edge\_distance\_hessian 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_distance_hessian (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    Eigen::Matrix< T, 12, 12 > & Hessian
) 
```




<hr>



### function edge\_edge\_distance\_type 

```C++
template<class T>
MUDA_GENERIC EdgeEdgeDistanceType muda::distance::edge_edge_distance_type (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1
) 
```




<hr>



### function edge\_edge\_distance\_unclassified 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_distance_unclassified (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    T & dist2
) 
```




<hr>



### function edge\_edge\_mollifier 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_mollifier (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    T eps_x,
    T & e
) 
```




<hr>



### function edge\_edge\_mollifier\_gradient 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_mollifier_gradient (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    T eps_x,
    Eigen::Vector< T, 12 > & g
) 
```




<hr>



### function edge\_edge\_mollifier\_hessian 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_mollifier_hessian (
    const Eigen::Vector< T, 3 > & ea0,
    const Eigen::Vector< T, 3 > & ea1,
    const Eigen::Vector< T, 3 > & eb0,
    const Eigen::Vector< T, 3 > & eb1,
    T eps_x,
    Eigen::Matrix< T, 12, 12 > & H
) 
```




<hr>



### function edge\_edge\_mollifier\_threshold 

```C++
template<class T>
MUDA_GENERIC void muda::distance::edge_edge_mollifier_threshold (
    const Eigen::Vector< T, 3 > & ea0_rest,
    const Eigen::Vector< T, 3 > & ea1_rest,
    const Eigen::Vector< T, 3 > & eb0_rest,
    const Eigen::Vector< T, 3 > & eb1_rest,
    T & eps_x
) 
```




<hr>



### function point\_edge\_ccd 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_edge_ccd (
    const Eigen::Matrix< T, 2, 1 > & x0,
    const Eigen::Matrix< T, 2, 1 > & x1,
    const Eigen::Matrix< T, 2, 1 > & x2,
    const Eigen::Matrix< T, 2, 1 > & d0,
    const Eigen::Matrix< T, 2, 1 > & d1,
    const Eigen::Matrix< T, 2, 1 > & d2,
    T eta,
    T & toc
) 
```




<hr>



### function point\_edge\_ccd 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_edge_ccd (
    Eigen::Matrix< T, 3, 1 > p,
    Eigen::Matrix< T, 3, 1 > e0,
    Eigen::Matrix< T, 3, 1 > e1,
    Eigen::Matrix< T, 3, 1 > dp,
    Eigen::Matrix< T, 3, 1 > de0,
    Eigen::Matrix< T, 3, 1 > de1,
    T eta,
    T thickness,
    int max_iter,
    T & toc
) 
```




<hr>



### function point\_edge\_ccd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_edge_ccd_broadphase (
    const Eigen::Matrix< T, 2, 1 > & p,
    const Eigen::Matrix< T, 2, 1 > & e0,
    const Eigen::Matrix< T, 2, 1 > & e1,
    const Eigen::Matrix< T, 2, 1 > & dp,
    const Eigen::Matrix< T, 2, 1 > & de0,
    const Eigen::Matrix< T, 2, 1 > & de1,
    T dist
) 
```




<hr>



### function point\_edge\_ccd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_edge_ccd_broadphase (
    const Eigen::Matrix< T, 3, 1 > & p,
    const Eigen::Matrix< T, 3, 1 > & e0,
    const Eigen::Matrix< T, 3, 1 > & e1,
    const Eigen::Matrix< T, 3, 1 > & dp,
    const Eigen::Matrix< T, 3, 1 > & de0,
    const Eigen::Matrix< T, 3, 1 > & de1,
    T dist
) 
```




<hr>



### function point\_edge\_cd\_broadphase 

```C++
template<typename T, int dim>
MUDA_GENERIC bool muda::distance::point_edge_cd_broadphase (
    const Eigen::Matrix< T, dim, 1 > & x0,
    const Eigen::Matrix< T, dim, 1 > & x1,
    const Eigen::Matrix< T, dim, 1 > & x2,
    T dist
) 
```




<hr>



### function point\_edge\_distance 

```C++
template<class T, int dim>
MUDA_GENERIC void muda::distance::point_edge_distance (
    const Eigen::Vector< T, dim > & p,
    const Eigen::Vector< T, dim > & e0,
    const Eigen::Vector< T, dim > & e1,
    T & dist2
) 
```




<hr>



### function point\_edge\_distance\_gradient 

```C++
template<class T, int dim>
MUDA_GENERIC void muda::distance::point_edge_distance_gradient (
    const Eigen::Vector< T, dim > & p,
    const Eigen::Vector< T, dim > & e0,
    const Eigen::Vector< T, dim > & e1,
    Eigen::Vector< T, dim *3 > & grad
) 
```




<hr>



### function point\_edge\_distance\_hessian 

```C++
template<class T, int dim>
MUDA_GENERIC void muda::distance::point_edge_distance_hessian (
    const Eigen::Vector< T, dim > & p,
    const Eigen::Vector< T, dim > & e0,
    const Eigen::Vector< T, dim > & e1,
    Eigen::Matrix< T, dim *3, dim *3 > & Hessian
) 
```




<hr>



### function point\_edge\_distance\_type 

```C++
template<class T, int dim>
MUDA_GENERIC PointEdgeDistanceType muda::distance::point_edge_distance_type (
    const Eigen::Vector< T, dim > & p,
    const Eigen::Vector< T, dim > & e0,
    const Eigen::Vector< T, dim > & e1
) 
```




<hr>



### function point\_edge\_distance\_type 

```C++
template<class T, int dim>
MUDA_GENERIC PointEdgeDistanceType muda::distance::point_edge_distance_type (
    const Eigen::Vector< T, dim > & p,
    const Eigen::Vector< T, dim > & e0,
    const Eigen::Vector< T, dim > & e1,
    T & ratio
) 
```




<hr>



### function point\_edge\_distance\_unclassified 

```C++
template<class T>
MUDA_GENERIC void muda::distance::point_edge_distance_unclassified (
    const Eigen::Vector< T, 3 > & p,
    const Eigen::Vector< T, 3 > & e0,
    const Eigen::Vector< T, 3 > & e1,
    T & dist2
) 
```




<hr>



### function point\_point\_ccd 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_point_ccd (
    Eigen::Matrix< T, 3, 1 > p0,
    Eigen::Matrix< T, 3, 1 > p1,
    Eigen::Matrix< T, 3, 1 > dp0,
    Eigen::Matrix< T, 3, 1 > dp1,
    T eta,
    T thickness,
    int max_iter,
    T & toc
) 
```




<hr>



### function point\_point\_ccd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_point_ccd_broadphase (
    const Eigen::Matrix< T, 3, 1 > & p0,
    const Eigen::Matrix< T, 3, 1 > & p1,
    const Eigen::Matrix< T, 3, 1 > & dp0,
    const Eigen::Matrix< T, 3, 1 > & dp1,
    T dist
) 
```




<hr>



### function point\_point\_distance 

```C++
template<class T, int dim>
MUDA_GENERIC void muda::distance::point_point_distance (
    const Eigen::Vector< T, dim > & a,
    const Eigen::Vector< T, dim > & b,
    T & dist2
) 
```




<hr>



### function point\_point\_distance\_gradient 

```C++
template<class T, int dim>
MUDA_GENERIC void muda::distance::point_point_distance_gradient (
    const Eigen::Vector< T, dim > & a,
    const Eigen::Vector< T, dim > & b,
    Eigen::Vector< T, dim *2 > & grad
) 
```




<hr>



### function point\_point\_distance\_hessian 

```C++
template<class T, int dim>
MUDA_GENERIC void muda::distance::point_point_distance_hessian (
    const Eigen::Vector< T, dim > & a,
    const Eigen::Vector< T, dim > & b,
    Eigen::Matrix< T, dim *2, dim *2 > & Hessian
) 
```




<hr>



### function point\_point\_distance\_type 

```C++
template<class T, int dim>
MUDA_GENERIC PointPointDistanceType muda::distance::point_point_distance_type (
    const Eigen::Vector< T, dim > & p0,
    const Eigen::Vector< T, dim > & p1
) 
```




<hr>



### function point\_point\_distance\_unclassified 

```C++
template<class T>
MUDA_GENERIC void muda::distance::point_point_distance_unclassified (
    const Eigen::Vector< T, 3 > & p0,
    const Eigen::Vector< T, 3 > & p1,
    T & dist2
) 
```




<hr>



### function point\_triangle\_ccd 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_triangle_ccd (
    Eigen::Matrix< T, 3, 1 > p,
    Eigen::Matrix< T, 3, 1 > t0,
    Eigen::Matrix< T, 3, 1 > t1,
    Eigen::Matrix< T, 3, 1 > t2,
    Eigen::Matrix< T, 3, 1 > dp,
    Eigen::Matrix< T, 3, 1 > dt0,
    Eigen::Matrix< T, 3, 1 > dt1,
    Eigen::Matrix< T, 3, 1 > dt2,
    T eta,
    T thickness,
    int max_iter,
    T & toc
) 
```




<hr>



### function point\_triangle\_ccd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_triangle_ccd_broadphase (
    const Eigen::Matrix< T, 3, 1 > & p,
    const Eigen::Matrix< T, 3, 1 > & t0,
    const Eigen::Matrix< T, 3, 1 > & t1,
    const Eigen::Matrix< T, 3, 1 > & t2,
    const Eigen::Matrix< T, 3, 1 > & dp,
    const Eigen::Matrix< T, 3, 1 > & dt0,
    const Eigen::Matrix< T, 3, 1 > & dt1,
    const Eigen::Matrix< T, 3, 1 > & dt2,
    T dist
) 
```




<hr>



### function point\_triangle\_cd\_broadphase 

```C++
template<typename T>
MUDA_GENERIC bool muda::distance::point_triangle_cd_broadphase (
    const Eigen::Matrix< T, 3, 1 > & p,
    const Eigen::Matrix< T, 3, 1 > & t0,
    const Eigen::Matrix< T, 3, 1 > & t1,
    const Eigen::Matrix< T, 3, 1 > & t2,
    T dist
) 
```




<hr>



### function point\_triangle\_distance 

```C++
template<class T>
MUDA_GENERIC void muda::distance::point_triangle_distance (
    const Eigen::Vector< T, 3 > & p,
    const Eigen::Vector< T, 3 > & t0,
    const Eigen::Vector< T, 3 > & t1,
    const Eigen::Vector< T, 3 > & t2,
    T & dist2
) 
```




<hr>



### function point\_triangle\_distance\_gradient 

```C++
template<class T>
MUDA_GENERIC void muda::distance::point_triangle_distance_gradient (
    const Eigen::Vector< T, 3 > & p,
    const Eigen::Vector< T, 3 > & t0,
    const Eigen::Vector< T, 3 > & t1,
    const Eigen::Vector< T, 3 > & t2,
    Eigen::Vector< T, 12 > & grad
) 
```




<hr>



### function point\_triangle\_distance\_hessian 

```C++
template<class T>
MUDA_GENERIC void muda::distance::point_triangle_distance_hessian (
    const Eigen::Vector< T, 3 > & p,
    const Eigen::Vector< T, 3 > & t0,
    const Eigen::Vector< T, 3 > & t1,
    const Eigen::Vector< T, 3 > & t2,
    Eigen::Matrix< T, 12, 12 > & Hessian
) 
```




<hr>



### function point\_triangle\_distance\_type 

```C++
template<class T>
MUDA_GENERIC PointTriangleDistanceType muda::distance::point_triangle_distance_type (
    const Eigen::Vector< T, 3 > & p,
    const Eigen::Vector< T, 3 > & t0,
    const Eigen::Vector< T, 3 > & t1,
    const Eigen::Vector< T, 3 > & t2
) 
```




<hr>



### function point\_triangle\_distance\_unclassified 

```C++
template<class T>
MUDA_GENERIC void muda::distance::point_triangle_distance_unclassified (
    const Eigen::Vector< T, 3 > & p,
    const Eigen::Vector< T, 3 > & t0,
    const Eigen::Vector< T, 3 > & t1,
    const Eigen::Vector< T, 3 > & t2,
    T & dist2
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/muda/ext/geo/distance/ccd.h`

