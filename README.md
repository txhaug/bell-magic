# Scalable measures of magic for quantum computers
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
