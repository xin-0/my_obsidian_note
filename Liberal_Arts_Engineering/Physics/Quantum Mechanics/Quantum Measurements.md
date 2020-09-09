## [[Quantum Mechanics Postulates#Postulate 3|Postulate]]

<br/>
<br/>

## Remark
1. the completeness equation express the fact that:
	$$1=p(m)=\sum_m{\bra\psi M_m^\dagger M_m\ket\psi}$$
2. Since a measurement device is a larger quantum mechanical system, some argues that Postulate 3 can be derived from Postualte 2. The [[Quantum Mechanics Unsolved Questions|disagreement]] remains unsettled.
<br/>
<br/>
## Examples
1. measurement in computational basis:
$$M_0=\ket0\bra0,M_1=\ket1\bra1$$

<br/>
<br/>

## Measurements
### - Projective measurements
---
projective measurement is described by an observable, $M$, a [[Hermitian]] operator on the state space of the system being observed. The observable has a spectral decomposition,
$$M=\sum_m{mP_m}$$
$P_m:$ projector onto the eigenspace of $M$ with eigenvalue $m$
$m:$ possible outcomes of the observable

Probability of getting result $m$ by measuring on sate $\ket\psi$:
$$p(m)=\bra\psi P_m\ket\psi$$

Given that outcome $m$ occured, the state immediately after the measurement is:
$${P_m\ket\psi\over \sqrt {p(m)}}$$

#### Remark:
1. When measurement in postulate, in addition to satisfying $\sum_m{M_m^\dagger M_m=I}$, also satisfy that $M_m$ are orthognal projectors, i.e. $M_m$ are Hermitian. Postulate reduce to a projective measurement.

#### Properties:
1. Expectation easily calculate:
	$$\begin{align} 
  E(M) & = \sum_m{mp(m)} \\
       & = \sum_m{m\bra\psi P_m\ket\psi} \\
	   & = \bra\psi \sum_m mP_m\ket\psi \\
	   & = \bra\psi M\ket\psi
  \end{align}$$
  Thus $\bra\psi M\ket\psi$ is often written as $\braket M$  
1. Standard Deviation:
	Genera Case:
	$$\begin{align}
	[\Delta (M)]^2 & = \braket {(M-\braket M )^2} \\
				   & = \braket {M^2}  - \braket M^2
	\end{align}$$
#### Spin measurement along axis $\vec v$:
$\vec v$ is a three-dimensional unit vector, the measurement operator is:
$$\vec v \vec \sigma=v_1 \sigma_1+v_2 \sigma_2+v_3 \sigma_3$$
where $\sigma_1, \sigma_2,\sigma_3$ are [[Pauli Matrices]]
<br/>
<br/>
##  POVM

Positive Operator-Valued Measure, a math tool. Useful for experiments where the systems are only measured for once and we don't care about the post state.
### Definition
> Suppose a measurement on quantum state $\ket\psi$ is described by measurement operators $\{M_m\}$. POVM is defined as 
> $$E_m=M_m^\dagger M_m$$
> $E_m$ are __POVM elements__. $\{E_m\}$ is POVM.
> Immediately we have:
> - $p(m)=\bra\psi E_m\ket\psi$
> - $\sum_m E_m=I$

### Remark
- Only when $M_m=P_m$, i.e. measurement operators are projectors, $E_m$ is the same as measurement operator:
	- $$E_m=M_m^\dagger M_m=P_m^\dagger P_m=P_m=M_m$$