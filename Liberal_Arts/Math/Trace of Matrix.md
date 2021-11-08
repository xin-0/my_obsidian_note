# Definition
- General:
	$$tr(A)\equiv\sum_i A_{ii}$$

- in quantum mechanic:
	$$tr(A) = \sum_n{\braket{n|A|n}}$$
	where $A$ is an arbitrary operator and the sum is over a set of basis vectors $\{ \ket n \}$
	This definition is related to the invariance property over different basis

# Properties
## 1. Cyclic
$$tr(ABC)=tr(BCA)=tr(CAB)$$

## 2. Linear
$$tr(A+B)=tr(A)+tr(B)$$
$$tr(\mathit z A)=\mathit z \cdot tr(A) \qquad \mathit z\in \Bbb C$$

## 3. Invariance
- Trace is invariant under the unitary similarity transformation: $A\rightarrow UAU^\dagger$:
	$$tr(UAU^\dagger)=tr(U^\dagger UA)=tr(A)$$
- Trace is invariant under change in basis
### _Application in [[Quantum Mechanics]]_
Suppose $\ket \psi$ is a unit vector, use the Gram–Schmidt procedure to extend $\ket \psi$ to an orthomormal basis $\ket i$, which start with $\ket \psi$.
Then for an arbitrary operator $A$:
$$\begin{align}
tr(A\ket\psi\bra\psi)&=\sum_i{\bra{i} \left( A\ket\psi\bra\psi\right)\ket{i}} \\
                     &=\sum_i{\bra{i}A\ket\psi\braket{\psi|i}} \\
					 &=\braket{\psi|A|\psi}
\end{align}$$

# Partial Trace
## Definition
$$tr_B(\ket{a_1}\bra{a_2}\otimes\ket{b_1}\bra{b_2})\equiv\ket{a_1}\bra{a_2}tr(\ket{b_1}\bra{b_2})$$
where $\ket{a_1}, \ket{a_2}$ are any two vectors in the state space of $A$ and $\ket{b_1}, \ket{b_2}$ are any two vectors in the state space of $B$.

## Remark
- $\begin{align} tr_B(\ket{a_1b_1}\bra{a_2b_2}) & =tr_B(\ket{a_1}\bra{a_2}\otimes\ket{b_1}\bra{b_2})=\ket{a_1}\bra{a_2}tr(\ket{b_1}\bra{b_2}) \\ & = \ket{a_1}\bra{a_2}\braket{b_2|b_1}\end{align}$
	- e.g: $tr_2(\ket{00}\bra{11})=\ket 0 \bra 1 \braket{1|0}=0$