# Definition
$$
\sigma_1\equiv\sigma_x\equiv X \equiv \begin{bmatrix}0&1\\1&0\end{bmatrix}\\   \sigma_2\equiv\sigma_y\equiv Y\equiv\begin{bmatrix}0&-i\\i&0\end{bmatrix} \qquad \sigma_3\equiv \sigma_z\equiv Z \equiv \begin{bmatrix}1&0\\0&-1\end{bmatrix}$$

$X$: bit flip
$Z$: phase flip
Sometimes also include $\sigma_0\equiv I\equiv\begin{bmatrix}1&0\\0&1\end{bmatrix}$

# Basic properties
- Pauli Matrices are [[Hermitian]]
# Eigenvalue decomposition
## Eigenvalue
There are two eigenvalues. $\lambda_+=1,\lambda_-=-1$ for all ${\sigma_x,\sigma_y,\sigma_z}$. Thus pauli matrices can be decomposed as: $\sigma=U\Lambda U^\dagger$, where $\Lambda=\begin{bmatrix}1&0\\0&-1\end{bmatrix}$

## Eigenvector
Since $\sigma_z=\Lambda=\begin{bmatrix}1&0\\0&-1\end{bmatrix}$, $\sigma_x$ and $\sigma_y$ can be decomposed respect to $\sigma_z$:
$$\sigma_x=\begin{bmatrix}{1\over\sqrt{2}}&{1\over\sqrt{2}}\\{1\over\sqrt{2}}&-{1\over\sqrt{2}}\end{bmatrix}
\begin{bmatrix}1&0\\0&-1\end{bmatrix}\begin{bmatrix}{1\over\sqrt{2}}&{1\over\sqrt{2}}\\{1\over\sqrt{2}}&-{1\over\sqrt{2}}\end{bmatrix}
$$
$$\sigma_y=\begin{bmatrix}{i\over\sqrt{2}}&{1\over\sqrt{2}}\\{-i\over\sqrt{2}}&{1\over\sqrt{2}}\end{bmatrix}
\begin{bmatrix}1&0\\0&-1\end{bmatrix}\begin{bmatrix}{-i\over\sqrt{2}}&{i\over\sqrt{2}}\\{1\over\sqrt{2}}&{1\over\sqrt{2}}\end{bmatrix}$$
Then we get two identities:
- $X=HZH$
- $Y=(HSX)Z(HSX)^\dagger$, where $S$ is [[Phase Gate|phase gate]].
  
 ### remark
- $Y=(HSX)Z(HSX)^\dagger=HSXZXS^\dagger H=-HSZS^\dagger H$