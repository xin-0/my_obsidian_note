# Definiton
- mathematically equivalent to state vector in describing [[Quantum Mechanics]]
- convenient when state is not completely known
- definition:
$$\rho\equiv\sum_i{p_i\ket{\psi_i}\bra{\psi_i}}$$

# Reformulated [[Quantum Mechanics Postulates|Postulates]] on Density Matrix
Mathematically equivalent to the description in terms of the [[Quantum Mechanics Postulates|state vector]]
1. State Space:
	- State Space for any isolated physical sysyem is a Hilbert Space
	- The system is completely described by its density operator
	- If a quantum system is in the state $\rho_i$ with probability $p_i$, then the density operator for the system is $\rho=\sum_i{p_i\rho_i}$
2. Evolution, for a closed quantum system
	 $$\rho=\sum_i{p_i\ket{\psi_i}\bra{\psi_i}} \xrightarrow{U}\sum_i{p_i U\ket{\psi_i}\bra{\psi_i}}U^\dagger=U\rho U^\dagger$$
3. Measurement
	- probability of getting result $m$
		$$p(m)=tr(M_m^\dagger M_m\rho)$$
	- density matrix of the system after obtaining measurement result $m$
		$$\rho_m={M_m\rho M_m^\dagger\over tr(M_m^\dagger M_m\rho)}$$
	- The measurement operators satisfy the completeness equation:
		$$\sum_m{M_m^\dagger M_m}=I$$
4. State Space of a composite physical system
	$$\otimes_i\rho_i$$
# Pure state and mixed state
A quantum system whose state $\ket \psi$ is known exactly is said to be in a pure state.
In this case the density operator is simply $\rho = \ket \psi \bra \psi$.
Otherwise $\rho$ is in a mixed state.
## General type of states
Mixtrue of pure states:
$$\rho=\sum_{k=1}^N{p_k\ket{\psi_k}\bra{\psi_k}}$$
## pure state
It is when $N=1$, thus we have:
$$tr(\rho^2)=1$$
## mixed state

It is when $N>1$, and thus: 
$$tr(\rho^2)<1$$

# Properties
## Characterization of density operators
### Theorem
An operator $\rho$ is the density operator associated to some ensemble $\{p_i, \ket{\psi_i}\}$ if and only if
1. Trace Condition: $\rho$ has trace equal to one
2. Positivity Condition: $\rho$ is a positive operator

# Non-uniqueness of the ensemble
==Different ensembles of quantum states may give rise to the same density matrix==
eigenvalues and eigenvectors of a density matrix does NOT possess special significance. Highly related to [[Quantum Information]] and [[Quatum Error Correction]]
Thus the qestion is: _what class of ensembles does give rise to a particular density matrix?_
## Unitary freedom in the ensemble for density matrices
Let $\ket{\tilde{\psi}_i}$ to be set of vectors that may not be normalized.  $\ket{\tilde{\psi}_i}$ generates density operator $\rho$, i.e. $\rho\equiv\sum_i{\ket{\tilde{\psi}_i}\bra{\tilde{\psi}_i}}$
### Theorem
The sets $\ket{\tilde{\psi}_i}$ and $\ket{\widetilde{\varphi}_j}$ generate the same density matrix if and only if
$$\ket{\tilde{\psi}_i}=\sum_j{u_{ij}}\ket{\widetilde{\varphi}_j}$$
Where $u_{ij}$ is a unitary matrix of complex numbers, with indices $i$ and $j$. Pad $0$ to the smaller set in $\ket{\tilde{\psi}_i}$ and $\ket{\widetilde{\varphi}_j}$ so that the two sets have the same number of elements.

### Consequence
- $\rho=\sum_i{p_i\ket{\psi_i}\bra{\psi_i}}=\sum_j{q_j\ket{\varphi_j}\bra{\varphi_j}}$ for normalized state $\ket{\psi_i},\ket{\varphi_j}$ and probability distribution $p_i,q_j$ if and only if
	$$\sqrt{p_i}\ket{\psi_i}=\sum_j{u_{ij}\sqrt{q_j}\ket{\varphi_j}}$$
	for some unitary matrix $u_{ij}$. and we may pad the smaller ensemble with entries having probability zero in order to make the two ensembles the same size.

# Reduced Density Operator
Density operator as a descriptive tool for _sub-systems_.
## Definition
Suppose we have physical systems $A$ and $B$, and the density operator describing the composite system is $\rho^{AB}$. The reduced density operator for system $A$ is defined as:
$$\rho^A\equiv tr_B(\rho^{AB})$$
where $tr_B$ is [[Trace of Matrix#Partial Trace#Definition|partial trace]] 

## Counter-intuitive Result
Consider a bell state
$$\ket \Psi={\ket{00}+\ket{11}\over \sqrt{2}}$$
The density operator for the two qubit system is
$$\begin{align}\rho&=\ket \Psi \bra\Psi ={(\ket{00}+\ket{11})(\bra{00}+\bra{11})\over 2}\\ &={\ket{00}\bra{00}+\ket{00}\bra{11}+\ket{11}\bra{00} + \ket{11}\bra{11} \over 2} \end{align}$$
We can get the reduced density matrix of the sub-system for the first qubit
$$\begin{align}
  \rho^1 & =tr_2(\rho) \\
  		 & ={1\over2}\left[tr_2(\ket{00}\bra{00})+tr_2(\ket{00}\bra{11})+tr_2(\ket{11}\bra{00})+tr_2(\ket{11}\bra{11})\right] \\
		 & ={1\over2}\left({\ket 0 \bra 0 \braket{0|0}+\ket 0 \bra 1 \braket{1|0} +\ket 1 \bra 0 \braket{0|1}+\ket 1\bra 1 \braket{1|1}}\right) \\
		 & = { \ket 0 \bra 0 + \ket 1\bra 1 \over 2}
  \end{align}
$$
Surprisingly
$$tr(\rho^2)=1,tr((\rho^1)^2)<1$$
It is very interesting to see that the composite system is in pure state which is 'known exactly' whereas the sub-system is in mixed state.