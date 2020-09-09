# Definition
$$tr(A)\equiv\sum_i A_{ii}$$

# Properties
## 1. Cyclic
$$tr(AB)=tr(BA)$$

## 2. Linear
$$tr(A+B)=tr(A)+tr(B)$$
$$tr(\mathit z A)=\mathit z A \qquad \mathit z\in \Bbb C$$

## 3. Invariance
Trace is invariant under the unitary similarity transformation: $A\rightarrow UAU^\dagger$:
$$tr(UAU^\dagger)=tr(U^\dagger UA)=tr(A)$$

### Application in [[Quantum Mechanics]]
Suppose $\ket \psi$ is a unit vector, use the Gram–Schmidt procedure to extend $\ket \psi$ to an orthomormal basis $\ket i$, which start with $\ket \psi$.
Then for an arbitrary operator $A$:
$$\begin{align}
tr(A\ket\psi\bra\psi)&=\sum_i{\bra{i} \left( A\ket\psi\bra\psi\right)\ket{i}} \\
                     &=\sum_i{\bra{i}A\ket\psi\braket{\psi|i}} \\
					 &=\braket{\psi|A|\psi}
\end{align}$$