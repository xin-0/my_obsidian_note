## Postulate
> Quantum measurements are described by a collection $\{M_m\}$, _measurement operators_. These are operators acting on the state space of the system being measured. The index $m$ refers to the measurement outcomes that may occur in the experiment.
> If the state of the quantum system is $\mid \psi\rangle$ immediately before the measurement then:
> 1. the probability that result $m$ occurs is  given by:
> $$p(m)=\langle\psi\mid M_m^\dagger M_m\mid\psi\rangle$$
> 2. and the state of the system after the measurement is :
> $${M_m\mid\psi\rangle\over \sqrt{\langle\psi\mid M_m^\dagger M_m\mid\psi\rangle}}$$
> 3. The measurement operators satisfy the [[Completeness Relation|completeness equation]]:
> $$\sum_m {M_m^\dagger M_m}=I$$

## Remark
1. the completeness equation express the fact that:
	$$1=p(m)=\sum_m{\langle\psi\mid M_m^\dagger M_m\mid\psi\rangle}$$
2. Since a measurement device is a larger quantum mechanical system, some argues that Postulate 3 can be derived from Postualte 2. The [[Quantum Mechanics Unsolved Questions|disagreement]] remains unsettled.
	
	
## Examples
1. measurement in computational basis:
$$M_0=\mid0\rangle\langle0\mid,M_1=\mid1\rangle\langle1\mid$$

## Measurements
### Projective measurements
projective measurement is described by an observable, $M$, a [[Hermitian]] operator on the state space of the system being observed. The observable has a spectral decomposition,
$$M=\sum_m{mP_m}$$
$P_m:$ projector onto the eigenspace of $M$ with eigenvalue $m$
$m:$ possible outcomes of the observable

Probability of getting result $m$ by measuring on sate $\mid\psi\rangle$:
$$p(m)=\langle\psi\mid P_m\mid\psi\rangle$$

Given that outcome $m$ occured, the state immediately after the measurement is:
$${P_m\mid\psi\rangle\over \sqrt {p(m)}}$$

Remark:
1. When measurement in postulate, in addition to satisfying $\sum_m{M_m^\dagger M_m=I}$, also satisfy that $M_m$ are orthognal projectors, i.e. $M_m$ are Hermitian. Postulate reduce to a projective measurement.

__Properties__:
1. Expectation easily calculate:
	$$\begin{align} 
  E(M) & = \sum_m{mp(m)} \\
       & = \sum_m{m\langle\psi\mid P_m\mid\psi\rangle} \\
	   & = \langle\psi\mid \sum_m mP_m\mid\psi\rangle \\
	   & = \langle\psi\mid M\mid\psi\rangle
  \end{align}$$
  	Thus $\langle\psi\mid M\mid\psi\rangle$ is often written as $\langle M\rangle$  
1. Standard Deviation:
	Genera Case:
	$$\begin{align}
	[\Delta (M)]^2 & = \langle (M-\langle M \rangle)^2\rangle \\
				   & = \langle M^2 \rangle - \langle M \rangle^2
	\end{align}$$
### POVM measurements
Positive Operator-Valued Measure, a math tool. Useful for experiments where the systems are only measured for once and we don't care about the post state.
_Def:_
- positive mastrix
- adds to $I$
