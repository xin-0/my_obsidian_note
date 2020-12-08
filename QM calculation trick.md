# Matrix noncommute
## square
$(A-B)^2=A^2-AB-BA+B^2=A^2-\{A,B\}+B^2$
$(A+B)^2=A^2+\{A,B\}+B^2$
$(A-B)(A+B)=A^2+AB-BA-B^2=A^2-B^2+[A,B]$

# [[Completeness Relation]]
![[Completeness Relation]]

# [[Clifford Gates]]
## Exponentiate Pauli Tensor
### Identity 1
$R_x(\theta)\otimes I=e^{-i{\theta\over2}(X\otimes I)}$
_Proof_:
$$\begin{align}
left & = \left({\cos{\theta\over2}I-i\sin{\theta\over2}X}\right)\otimes I\\
     & = \cos{\theta\over2}I\otimes I-i\sin{\theta\over2}X\otimes I \\
\tag{taylor} right& = 1-i{\theta\over2}(X\otimes I)-\frac{({\theta\over2})^2(X\otimes I)^2}{2!}+i\frac{({\theta\over2})^3(X\otimes I)^3}{3!}+... \\
     & =  1-i{\theta\over2}(X\otimes I)-\frac{({\theta\over2})^2(X^2\otimes I^2)}{2!}+...+(-i)^n\frac{({\theta\over2})^n(X^n\otimes I^n)}{n!}+... \\
	 & = \left({1 - \frac{({\theta/2})^2}{2!} + ...+(-1)^n\frac{({\theta/2})^{2n}}{(2n)!}+...}\right)(I\otimes I)\\
	 & \qquad + (-i)\left({(\theta/2)-\frac{(\theta/2)^3}{3!}+...+(-1)^{2n+1}\frac{(\theta/2)^{2n+1}}{(2n+1)!}+...}\right)(X\otimes I) \\
	 & = \cos{\theta\over2}(I\otimes I)-i\sin{\theta\over2}(X\otimes I)
\end{align}$$
Thus $left=right$.
#### remark
We have this identity due to:
1. $\pm1$ eigenvalue for pauli matrices, $\sigma$, such that $e^{i\alpha\sigma}=\cos{\alpha}\cdot I+i\sin{\alpha}\cdot\sigma$
2. $\pm1$ eigenvalue for pauli matrices, $\sigma$, such that $\sigma^{2n}=I, \sigma^{2n+1}=\sigma$

Thus, it is reasonable to guess: $R_{\hat{n}}(\theta)\otimes I=e^{-i{\theta\over2}(\hat n \sigma\otimes I)}$