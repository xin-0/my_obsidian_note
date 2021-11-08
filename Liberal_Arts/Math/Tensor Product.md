# Basic
$\vec v = \begin{bmatrix} v_0 \\ v_1 \end{bmatrix}$
$\vec u = \begin{bmatrix} u_0 \\ u_1 \end{bmatrix}$

$\vec v\otimes\vec u= \begin{bmatrix} v_0\vec u \\ v_1\vec u \end{bmatrix}= \begin{bmatrix} v_0u_0 \\ v_0u_1\\v_1u_0\\v_1u_1 \end{bmatrix}$

![[tensor.png|300]]

# Properties

1. Associative on scalar
	$$z\left({\ket v \otimes\ket w}\right)=\left({}z\ket v\right)\otimes\ket w=\ket v \left({z\ket w}\right)$$
			
1. distributive on addition
	$$(\ket {v_1}+\ket {v_2})\otimes\ket w=\ket {v_1} \otimes\ket w + \ket {v_2}\otimes \ket w$$
	$$\ket v\otimes(\ket {w_1}+\ket{w_2})=\ket v \otimes\ket {w_1}+\ket v\otimes \ket{w_2}$$
	
3. $(A\otimes B)(\ket v \otimes \ket w)=A\ket v \otimes B \ket w$
4. Involving inner product
	$$\left({\sum_i{a_i\ket{v_i}\ket{w_i}},\sum_j{b_j\ket{v_j}\ket{w_j}}}\right)=\sum_{ij}{a_i^*b_j\braket{v_i|v_j}\braket{w_i|w_j}}$$
	
5. Distributive on transpose, complex conjugation, and adjoint operations
	$$(A\otimes B)^*=A^*\otimes B^*;(A\otimes B)^T=A^T\otimes B^T; (A\otimes B)^\dagger=A^\dagger\otimes B^\dagger$$
	
6. $U,V$ are unitaries $\implies U\otimes V$ is [[Unitary|unitary]]
7. $H, K$ are hermitians $\implies H\otimes K$ is [[Hermitian|hermitian]]
8. $A, B>0 \implies (A\otimes B)>0$ 
9. $P, J$ are projectors $\implies P\otimes J$ is projector

# Specific cases
## [[Hadamard Gate]]
$$H^{\otimes n}={1 \over \sqrt{2^n}}\sum_{x,y}{(-1)^{xy}\ket{x}\bra{y}}$$
