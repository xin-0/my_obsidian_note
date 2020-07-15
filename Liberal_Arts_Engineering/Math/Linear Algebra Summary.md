#### Vector properties
1. commutativity
2. associativity
3. distributivityofscalarmultiplication
4. distributivityofscalaraddition
5. Existence of additive identity
6. Existence of additive inverse

#### Matrix operation
1. commutative addition
2. non-commutative multiplication
3. distributive
4. associative

#### Linearity
def: 
$$L(x+y)=L(x)+L(y) $$
$$L(cx)=cL(x)$$

#### Conjugate, Transpose
##### Conjugate
 $(\overline{\vec v})_i=\overline v_i$
$\left(\overline{\mathbf M}\right)_{ij}=\overline{\mathbf M_{ij}}$
##### conjugate transpose
 $\left(\mathbf M^\dagger\right)_{ij}=\overline M_{ji}$

---
#### Inner Product
##### basic
$\vec v \cdot\vec w=\vec v^\dagger\vec w$
##### properties
$\vec v\cdot\vec w=\overline{\vec w\cdot\vec v}$
$\vec v \cdot\left(\mathbf M\vec w\right)=\left(\mathbf M^\dagger\vec v\right)\cdot\vec w$
##### Naive Def of Hilbert Space
vector space + well-ddefined inner product space
##### Vector Norm
 $\lVert\vec v\rVert=\sqrt{\vec v\cdot\vec v}$
##### Basis
Orthonormal basis:  each vector has norm one 1 and orthogonal to each other
Canonical basis: [[computational basis]] in quantum mechanics

##### Orthonormal Projection
$\mathbf P_{\vec v,\vec w}={1\over\lVert\vec w\rVert}\vec w \cdot \vec v$
 
 ---
#### Special Matrices
 
##### Identity Matrix 
$\Bbb 1$ or $I$
###### Definition
n by n matrix
$$\mathbb 1 M=M\Bbb 1=M \quad and\quad \Bbb 1 \vec v=\vec v$$

##### Unitary Matrix
###### Definition
$U$ such that
$$UU^\dagger=U^\dagger U=\Bbb 1$$
###### properties
- Preserve Inner Product
	- If $\vec w_1 =U\vec v_1\quad and \quad\vec w_2 =U\vec v_2$
	- then $\vec w_1\cdot\vec w_2=\vec v_1\cdot\vec v_2$
 