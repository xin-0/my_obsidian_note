# Definition
## Single-qubit
> if $U$ is a Clifford and $P$ is a Pauli, $UPU^\dagger$ is also a Pauli.
## Multi-qubit
>Unitary matrix that transform tensor product of Paulis into other tensor product of Paulis.
### example
CNOT:
$$CNOT_{j,k}(X\otimes I)CNOT_{j,k}=X\otimes X$$

# Non-Clifford Gates

## Single-qubit
$R_x(\theta),R_y(\theta),R_z(\theta)$
### Transformation
For an unitary $U$, we can show that:
$$UR_x(\theta)U^\dagger=e^{-i{\theta\over2}UXU^\dagger}$$
By conjugating this rotation by a Clifford, we can therefore transform it to the same rotation around another axis. $R_y(\theta), R_z(\theta)$ can be implemented using $R_x(\theta)+Clifford$

## Multi-qubit
conjugating with CNOT:
$$\begin{align}
CNOT_{j,k}(R_x(\theta)\otimes I)CNOT_{j,k} &=CNOT_{j,k}e^{-i{\theta\over2}(X\otimes I)}CNOT_{j,k}\\
&=e^{-i{\theta\over2}CNOT_{j,k}(X\otimes I)CNOT_{j,k}}\\
& = e^{-i{\theta\over2}(X\otimes X)}
\end{align}$$