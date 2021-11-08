# Theorem
>Suppose $\ket \psi$ is a ==pure state== of a composite system, $AB$. Then there exist ==orthonormal== bases $\{\ket{i_A}\}, \{\ket{i_B}\}$ for system $A,B$ respectively such that 
$$\ket\psi=\sum_i{\lambda_i\ket{i_A}\ket{i_B}}$$
where $\lambda_i\in\Bbb R^+$ and $\sum_i\lambda_i^2=1$ known as _Schmidt coefficient_.
$\{\ket{i_A}\}, \{\ket{i_B}\}$: _Schmidt Bases_
$i$: _Schmidt number_
## Proof
For an arbitrary pure state $\ket \psi$ in a composite system we have
$$\begin{align}
\ket \psi & = \sum_{jk}{a_{jk}\ket j \ket k}\\
		  & = \sum_{ijk}{u_{ji}d_{ii}v_{ik}\ket j \ket k}
\end{align}$$
Then define $\ket{i_A}\equiv \sum_j{u_{ji}\ket j}$, $\ket{i_B}\equiv \sum_k{v_{ik}\ket k}$ and $\lambda_i=d_{ii}$, it gives
$$\ket\psi=\sum_i{\lambda_i\ket{i_A}\ket{i_B}}$$

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

# Example
## Get Schmidt Decomposition
### Q1.
$${\ket{00}+\ket{01}+\ket{10}+\ket{11}\over2}$$
Do SVD, which is eigendecomposition in the case of a square matrix
$$\begin{align}
{1\over2}\begin{bmatrix}1 &1\\ 1 & 0\end{bmatrix} & = 
\begin{bmatrix}{1\over\sqrt{2}} & -{1\over\sqrt{2}}\\ {1\over\sqrt{2}} & {1\over\sqrt{2}} \end{bmatrix}\begin{bmatrix}1 &0\\ 0 & 0\end{bmatrix}
\begin{bmatrix}{1\over\sqrt{2}} & -{1\over\sqrt{2}}\\ {1\over\sqrt{2}} & {1\over\sqrt{2}} \end{bmatrix} \\
& = \begin{bmatrix} u_1, u_2\end{bmatrix} \begin{bmatrix}1 &0\\ 0 & 0\end{bmatrix} \begin{bmatrix} v_1^T\\ v_2^T\end{bmatrix}
\end{align}$$
Thus 
$\ket{0_A}= \ket 1 , \ket{1_A}=u_{01}\ket 0+u_{11} \ket 1$