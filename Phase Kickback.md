## Definition
>Kickback is where the eigenvalue added by a gate to a qubit is ‘kicked back’ into a different qubit via a controlled operation.


## General 
If we have an unitary $U$ and its eigenstate $\ket\psi$ with:
$$U\ket\psi=e^{i\theta}\ket\psi$$
 $controlled-U\equiv\begin{bmatrix} I & \\ & U \end{bmatrix}$ with control qubit $\ket c=\alpha\ket 0+\beta\ket1$ acting on target qubit $\ket\psi$, the control qubit will pick up the relative phase instead leaving the target qubit unchanged.
 $$\begin{align}
 C-U\ket{c\psi}
 	& = \alpha\ket{0\psi} + \beta\ket1U\ket\psi \\
	& = \alpha\ket{0\psi} + \beta e^{i\theta}\ket{1\psi} \\
	& = \left({\alpha\ket{0}+\beta e^{i\theta}\ket{1}}\right)\ket\psi
 \end{align}$$
 $\ket c$ as the control bit, pick up the phase.
 
 ## Example
### CNOT
When we apply $X$ on $\ket -$, $X\ket -=-\ket -$.
When the control bit is either $0$ or $1$, 
$$CNOT\ket{0-}=\ket{0-}$$
$$CNOT\ket{1-}=-\ket{1-}$$
Initial and final states only differ by a global phase.
When the control bit is in superposition:
$$\begin{align}
CNOT\ket{-+} & = CNOT\ket-{1\over\sqrt 2}(\ket -+\ket +) \\
             & = \ket-{1\over\sqrt 2}(\ket --\ket +) \\
			 & = \ket {--}\\
\end{align}$$