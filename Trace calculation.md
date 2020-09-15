# Example 1
Expectation value of operators can be expressed in term of projector
	$$\begin{align}
	\tag{1}\braket{O}_\psi & = \braket{\psi|O|\psi} \\
	\tag{2}                & = \braket{\psi|IO|\psi} \\
	\tag{3}                & = \braket{\psi|\left(\sum_n{\ket n \bra n} \right)O|\psi} \\
	\tag{4}                & = \sum_n{\braket{\psi|n}\braket{n|O|\psi}} \\
	\tag{5}                & = \sum_n{\braket{n|O|\psi}\braket{\psi|n}} \\
	\tag{6}                & = \sum_n{\braket{n|OP_\psi|n}} \\
	\tag{7}                & = tr(OP_\psi)
	\end{align}$$
	$(1):$ definition of expectation
	$(2):$ inserting identity
	$(3):$ using [[Completeness Relation]]
	$(4):$ the rest does not depend on $n$, thus can be move into or outside the summation
	$(5):$ $\braket{\psi|n}$ is a scalar, thus commutative, can be moved to the end.
	$(6):$ "definition" of projector, $\ket \psi \bra \psi$ is a projector onto $\ket\psi$
	$(7):$ definition of [[Trace of Matrix#Definition|trace]]

# Example 2
express probabilities and overlaps in terms of projector and trace, $\vert\braket{\phi|\psi}\vert^2=tr(\ket \phi \bra \phi P_\psi)=tr(P_\psi\ket \phi \bra \phi)$:
	$$\begin{align}
	\tag{} \vert\braket{\phi|\psi}\vert^2 & = \braket{\psi|\phi}\braket{\phi|\psi} \\
	\tag{1}          & = \braket{\psi|I|\phi}\braket{\phi|\psi} \\
	\tag{2} 		 & = \bra{\psi}\left(\sum_n{\ket n \bra n}\right)\ket \phi \braket{\phi|\psi} \\
	\tag{3}          & = \sum_n{\braket{\psi|n}\braket{n|\phi}\braket{\phi|\psi}} \\
	\tag{4}          & = \sum{\braket{n|\phi}\braket{\phi|\psi}\braket{\psi|n}} \\
	\tag{5}          & = tr(\ket \phi \braket{\phi|\psi}\bra \psi) \\
	\tag{6}          & = tr(\ket \phi \bra \phi P_\psi)
	\end{align}$$