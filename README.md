# Quantum Adder With Noise

(This was initially done for QOSF mentorship screening. The solution/codes in the python notebook is chosen as the best solution by QOSF team.)

Task 2 Noise, Noise, and More Noise 

One of the main challenges in quantum computing is the noise in current devices. In this task, you will create a simple noise generator and assess its effect. You can use any framework you like (Qiskit, Cirq, etc..)

Noise Model 

A standard way to represent the noise in a quantum circuit is through Pauli operators (x, y, z). Build a function with input ,  and QuantumCircuit where:

  → Probability of having a random Pauli operator acting on the qubit after a one-qubit gate 
  → Probability of having a random Pauli operator acting on the qubit after a two-qubit gate 
QuantumCircuit → Quantum circuit where the noise will be added 

The output should be the Quantum Circuit with Noise 

Gate Basis 

Quantum computers can implement only a set of gates that, with transformations, can represent any other possible gate. This set of gates is called the Gate Basis of the QPU. Build a function that transforms a general Quantum Circuit to the following gate basis: {CX,ID,RZ,SX,X}

Adding two numbers with a quantum computer

Build a function (quantum_sum) to add two numbers using the Draper adder algorithm. You will need the Quantum Fourier Transform (QFT). Many libraries offer a function to use it. For this task, you will need to build QFT from scratch.

Effects of noise on quantum addition 

Now, we can combine all the functions. Transform the circuit used in the quantum_sum to the gate basis and add noise. Use different levels of noise and analyze the results. 

How does the noise affect the results? 
Is there a way to decrease the effect of noise? 
How does the number of gates used affect the results? 

References:

[3] Quantum arithmetic with the Quantum Fourier Transform 
https://arxiv.org/pdf/1411.5949.pdf
