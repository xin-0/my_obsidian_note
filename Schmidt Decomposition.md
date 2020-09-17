# Theorem
Suppose $\ket \psi$ is a ==pure state== of a composite system, $AB$. Then there exist ==orthonormal== bases $\{\ket{i_A}\}, \{\ket{i_B}\}$ for system $A,B$ respectively such that 
$$\ket\psi=\sum_i{\lambda_i\ket{i_A}\ket{i_B}}$$
where $\lambda_i\in\Bbb R^+$ and $\sum_i\lambda_i^2=1$ known as _Schmidt number_.
$\{\ket{i_A}\}, \{\ket{i_B}\}$: _Schmidt Bases_

# Property
## Invariance of Schimdt number
Schmidt number is preserved under unitary transformations on system $A$ or system or
$B$ alone:
if $\ket \psi$ has schimdt decomposition
$$\sum_i\lambda_i\ket{i_A}\ket{i_B}$$
$U\ket \psi$ has schimdt decomposition, $U$ only acts on system $A$
$$\sum_i\lambda_i (U\ket{i_A})\ket{i_B}$$