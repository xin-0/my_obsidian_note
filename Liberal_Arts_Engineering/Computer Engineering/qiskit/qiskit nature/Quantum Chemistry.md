## Construct Hamiltonian
### Molecular Hamiltonians
$$\begin{align}
H &= -\sum_{i=1}^N{{1\over 2}\nabla^2_i}
    -\sum_{A=1}^M{{1\over 2M_A}\nabla^2_A} 
	-\sum_{i=1}^N{\sum_{A=1}^M{Z_A\over r_{iA}}}
	+\sum_{j>i}{1\over r_{ij}}
	+\sum_{B>A}{Z_AZ_B\over R_{AB}} \\
H &= \text{Elect KE }
	+\text{Nuclear KE }
	+\text{E-N coulomb}
	+\text{E-E coulomb}
	+\text{N-N coulomb}
\end{align}$$

Usually we are interested in the ground state $\ket\psi$ for the above hamiltonian, which is a solution to $$H\ket\psi=E\ket\psi$$ with the lowest energy $E_0$.

Knowing $E_0$ enables us to know reaction rate, etc for designing new drugs and materials.

#### Born–Oppenheimer approximation
One way to solve the question is Born–Oppenheimer approximation:
> It assumes the nucleai are fixed then in $H$
> $$\text{Nuclear KE=0}$$ $$\text{N-N coulomb = energy shift}$$

This method reduce the problem into "Problem of interacting electron" (still exponentially hard)

#### Distinguishability
- Qubits are distinguishable: $$\ket\psi=\ket {\chi_1}_1\ket {\chi_2}_2$$
	- qubit 1 in $\chi_1$ state
	- qubit 2 in $\chi_2$ state
- Electrons (Fermions) are indistinguishable particles. $$\ket{\psi}={1\over\sqrt{2}}(\ket {\chi_1}_1\ket {\chi_2}_2-\ket {\chi_2}_1\ket {\chi_1}_2)$$
	- always cannot tell a certain electron is in certain state
	- anti-symmetric "$-$": means if we exchange Particle $1\leftrightarrow 2$ $$\ket\psi\to-\ket\psi$$this is true for all fermions.
		- For $N$ fermions $$\ket\psi={1\over\sqrt{N!}}\begin{vmatrix}\ket{\chi_1}_1&\cdots & \ket{\chi_1}_N \\
		\vdots & \ddots & \vdots \\
		\ket{\chi_1}_N & \cdots & \ket{\chi_N}_N
		\end{vmatrix}$$The determinant above is called "Slater Determinant"


### Second Quantization Notation

### Fermion to qubit mappings

## Variational Quantum Algorithms

### why works

### popular variational wavefuntions

### open challenges