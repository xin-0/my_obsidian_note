#Quantum_Mechanic #Model_Reality_Correlation 

## Postulate 1
Key idea: State Space in Math <--> Physical World
> The __state space__ of an isolated physical system is a Hilbert Space. The system is completely described by state vector, an unit vector in the state space

### Remark:
- Qubit is a math object.
- we need such postulate since QM does not tell us the state space of the system.
<br/>
<br/>

## Postulate 2
Key idea: how quantum mechanical systems evolve in time
> The evolution of a __closed__ quantum system is described by a __unitary transformation__. If the system is in state $\mid\psi\rangle$ at $T=t_1$ and in state $\mid\psi^{'}\rangle$ at $T=t_2$, then two states are related with an unitary operator $U$ by:
> $$ \mid\psi^{'}\rangle = U\mid\psi\rangle$$
> where $U$ only depends on $t_1$ and $t_2$.

### Remark:
1.  $U$ can be any unitary that can be realized in realistic systems, e.g.:
	- [[Pauli Matrices]]
	- [[Hadamard Gate]]
2.  "Closed": it is not insteracting with other systems

__Revied Version__ of Postulate 2: for _continuous time_
> A closed quantum system evolve in time according to Schrödinger equation,
> $$i\hbar{d\mid\psi\rangle\over dt}=H\mid\psi\rangle$$
- $H$ is [[Hamiltonian]], a Hermitian operator
<br/>
<br/>

## Postulate 3
> Quantum measurements are described by a collection $\{M_m\}$, _measurement operators_. These are operators acting on the state space of the system being measured. The index $m$ refers to the measurement outcomes that may occur in the experiment.
> If the state of the quantum system is $\mid \psi\rangle$ immediately before the measurement then:
> 1. the probability that result $m$ occurs is  given by:
> $$p(m)=\langle\psi\mid M_m^\dagger M_m\mid\psi\rangle$$
> 2. and the state of the system after the measurement is :
> $${M_m\mid\psi\rangle\over \sqrt{\langle\psi\mid M_m^\dagger M_m\mid\psi\rangle}}$$
> 3. The measurement operators satisfy the [[Completeness Relation|completeness equation]]:
> $$\sum_m {M_m^\dagger M_m}=I$$

### Remark:
- [[Quantum Measurements]]