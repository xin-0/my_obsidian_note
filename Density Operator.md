# Definiton
- mathematically equivalent to state vector in describing [[Quantum Mechanics]]
- convenient when state is not completely known
- definition:
$$\rho\equiv\sum_i{p_i\ket{\psi_i}\bra{\psi_i}}$$

# Reformulated [[Quantum Mechanics Postulates|Postulates]] on Density Matrix
1. Evolution:
	 $$\rho=\sum_i{p_i\ket{\psi_i}\bra{\psi_i}} \xrightarrow{U}\sum_i{p_i U\ket{\psi_i}\bra{\psi_i}}U^\dagger=U\rho U^\dagger$$
2. Measurement:
	- probability of getting result $m$
		$$p(m)=tr(M_m^\dagger M_m\rho)$$
	- density matrix of the system after obtaining measurement result $m$
		$$\rho_m={M_m\rho M_m^\dagger\over tr(M_m^\dagger M_m\rho)}$$
		
# Pure state and mixed state
