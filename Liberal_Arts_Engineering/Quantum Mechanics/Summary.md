# Math Postulates
1. To every physical system there is a function $\Psi$ ascribe to and defining the state.
	- Physical Sytem: a free particle in QM
2. Composite system lives in a space that is the tensor product of two individual Hilbert spaces
3. Every observable is represented by eigenvalues of a Hermitian oprator in Hilbert Space
4. Quantum operations and time evolution of a quantum state are represented by unitary operator on the Hilbert 
	- consequence of Schordinger's Equation


# notation and computation:
## Basic:
$\mid\psi\rangle=v\in\Bbb {C} ^n$, $\mid\phi\rangle=w\in\Bbb {C} ^n$
- $\langle\psi\mid = \mid\psi\rangle^\dagger=v^\dagger$
- inner product: $\langle\psi\mid\phi\rangle=v^\dagger w$
- Measure $\mid\psi\rangle$ in $\mid\phi\rangle$: yields$\mid\phi\rangle$ with probability $\vert \langle\psi\mid\phi\rangle\vert^2$

## Hamiltonian
Harmonic Oscillator: 
- $H=\sum_k{E_k\mid\psi_k\rangle\langle\psi_k\mid}$
- $\langle\psi_j\mid\psi_k\rangle=\delta_{j,k}$ --> Orthonormal
- $\{\mid\psi_k\rangle\}$ form a basis of infinite dimension $\mid\psi_k\rangle$ -->$\mid k\rangle$

## Operations & Observables
1. logic gates $\equiv$ unitary matrices $\equiv$ change of basis:
$$U=\sum_k{\mid\psi_k\rangle\langle k\mid}$$


2. readout $\equiv$ measurement operators $\equiv$ Hermitians
$$A=\sum_k{r_k\mid\psi_k\rangle\langle \psi_k\mid},\quad r_k\in\Bbb R$$
