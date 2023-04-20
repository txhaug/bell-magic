# Measuring magic with quantum computers

Code for "Scalable measures of magic resource for quantum computers" by Tobias Haug, M.S. Kim. (PRX Quantum 4, 010301)

https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.4.010301

Magic quantifies the distance of a quantum state to the set of stabilizer states, a class of states that can be efficiently computed with classical computers.
Magic is a necessary condition for quantum advantage and an important resource for fault-tolerant quantum computers.
This code provides a scalable measurement method to measure Bell magic of quantum states prepared on a quantum computer.

Bell magic is measured by creating two copies of a state and measuring it in the Bell basis. Various types of quantum states are supported.
Simulates the circuit and measurement with qiskit for variable types of circuit, number of measurements and depolarization error.
Error mitigation scheme based on a complementary purity estimation is included.

Can run stabilizer circuit + T-gates, magic states, magic states + stabilizer circuit, etc. 
For n_samples=0, runs exact statevector simulator for infinite samples, else n_samples>0 qasm simulator with n_samples measurements.
Instead of qasm simulator, can be easily run on IBMQ hardware (or any other quantum computer).
Measurement method is scalable to any number of qubits, beyond what qiskit can simulate.

Requirements:
- qiskit
- numpy
