# Quantum-Teleportation-using-QASM
Open Quantum Assembly Language is an intermediate representation for quantum instructions.

Quantum teleportation is designed to send qubits between two entities. 

There exists a theorem in quantum mechanics which states that you cannot simply make an exact copy of an unknown quantum state. (the no-cloning theorem). If we read out a quantum state, the superposition and entanglement is destroyed. And still we can teleport quantum states between two qubits. 

Quantum teleportation is totally real.

http://www.physics.umd.edu/grt/taj/623e/CanaryTeleportation.pdf

https://arxiv.org/pdf/quant-ph/0604027.pdf

Consider two people Alice and Bob. Alice is going to transfer a message qubit to Bob.The Qiskit textbook uses this analogy.

STEPS FOR QUANTUM TELEPORTATION: (Requires 3 qubits and 2 classical bits.)
1. Prepare the quantum state Q_message. It could be any arbitrary state. Here, U gate.
2. Entangle the other two qubits. Q_Alice and Q_Bob. Alice is going to entangle the two qubits and will keep one of them --> Q_Alice. The other one she will send to Bob.
3. Send the entangled qubit to Bob.
4. Bell Measurement. Alice still has Q_message and Q_Alice. Bell measurement is a quantum mechanic measurement that determines which of the Bell states the qubits belong to. 
5. Recreate the quantum state.
