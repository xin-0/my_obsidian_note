# Theorem
>Suppose $\ket \psi$ is a ==pure state== of a composite system, $AB$. Then there exist ==orthonormal== bases $\{\ket{i_A}\}, \{\ket{i_B}\}$ for system $A,B$ respectively such that 
$$\ket\psi=\sum_i{\lambda_i\ket{i_A}\ket{i_B}}$$
where $\lambda_i\in\Bbb R^+$ and $\sum_i\lambda_i^2=1$ known as _Schmidt number_.
$\{\ket{i_A}\}, \{\ket{i_B}\}$: _Schmidt Bases_

# Propositions
## Invariance of Schimdt number
Schmidt number is preserved under unitary transformations on system $A$ or system or
$B$ alone:
if $\ket \psi$ has schimdt decomposition
$$\sum_i\lambda_i\ket{i_A}\ket{i_B}$$
$U\ket \psi$ has schimdt decomposition, $U$ only acts on system $A$
$$\sum_i\lambda_i (U\ket{i_A})\ket{i_B}$$

## Product State
- $\ket\psi$ of a composite system $AB$ is a product state $\iff$ it has Schmidt number $1$.
- $\ket \psi$ is a product state $\iff$ $\rho^A$ (and thus $\rho^B$) are pure states

# Purification
>For any given state $\rho^A$ of a quantum system $A$. It is possible to introduce a _reference _ system $R$ and define a pure state $\ket{AR}$ s.t. $$\rho^A=tr_R(\ket{AR}\bra{AR})$$
>we can do this by define $$\ket{AR}\equiv\sum_i\sqrt{p_i}\ket{i^A}\ket{i^R}$$

Since the process can turn a mixed state, $\rho^A$,  into a pure state $\ket{AR}$. Such procedure is called purification.