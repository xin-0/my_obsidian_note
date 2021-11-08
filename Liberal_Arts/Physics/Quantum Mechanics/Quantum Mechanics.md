# Foundation
-  [[Quantum Mechanics Postulates]]
# notation and computation
## Basic
$\ket\psi=v\in\Bbb {C} ^n$, $\ket\varphi=w\in\Bbb {C} ^n$
- $\bra\psi = \ket\psi^\dagger=v^\dagger$
- inner product: $\braket{\psi\mid\varphi}=v^\dagger w$
- Measure $\ket\psi$ in $\ket\varphi$: yields$\ket\varphi$ with probability $\vert \braket{\psi\mid\varphi}\vert^2$
- 
## [[Hamiltonian]]
$\equiv$ __bais__
Harmonic Oscillator: 
- $H=\sum_k{E_k\ket{\psi_k}\bra{\psi_k}}$
- $\braket{\psi_j\mid\psi_k}=\delta_{j,k}$ --> Orthonormal
- $\{\ket{\psi_k}\}$ form a basis of infinite dimension $\ket{\psi_k}$ -->$\ket k$

Z-basis:
- $Z=\ket 0 \bra 0+\ket 1 \bra 1$

## Operations & Observables
1. logic gates $\equiv$ [[Unitary]] matrices $\equiv$ change of basis:
$$U=\sum_k{\ket{\psi_k}\bra k}$$


2. readout $\equiv$ measurement operators $\equiv$ [[Hermitian]]
$$A=\sum_k{r_k\ket{\psi_k} \bra{\psi_k}},\quad r_k\in\Bbb R$$

3. average experimental outcome $\equiv$ Probability [[Expectation]] $\equiv$ "sandwich" operator
$$\bra\phi A \ket\phi=\sum _kr_k\vert\braket{\psi_k\mid\phi}\vert^2$$

## Some Unitaries
* $X= \begin{bmatrix}0&1\\1&0\end{bmatrix}$
* [[Hadamard Gate]]
* [[Phase Gate]] 
* [[Pauli Matrices]]

## [[Bloch Sphere]]


## Multi-qubit states & operations
Kronecker Products:
$$A\otimes B$$

- $(A\otimes B)(C\otimes D)=(AC)\otimes(BD)$

## State Decomposition
To convert a state $\ket\varphi$ into $\{\ket{\psi_k}, k=0,1,...\}$ basis:
$$\ket\varphi=\sum_k{\braket{\psi_k\mid\varphi}\ket{\psi_k}}$$

 ### Remarks
 - measurement in lab vs measurement in theory