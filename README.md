# Qiskit Quantum Circuits

Quantum computing experiments and implementations using **Qiskit**, **IBM Quantum**, and Python.

This repository contains hands-on experiments exploring quantum states, quantum circuits, visualization, simulation, and execution on real quantum hardware.

---

## Experiments

### 01. Quantum Entanglement — Bell State

This experiment demonstrates the preparation and measurement of a two-qubit Bell state using Qiskit.

The experiment includes:

- Construction of the Bell state

  $$
  |\Phi^+\rangle =
  \frac{|00\rangle + |11\rangle}{\sqrt{2}}
  $$

- Statevector simulation and theoretical probability analysis
- 1024-shot ideal simulation
- Hardware-specific circuit transpilation
- Execution on a real IBM Quantum processor
- Comparison between ideal simulation and real hardware results
- Observation of hardware noise and measurement errors

The Bell-state circuit was executed on the IBM Quantum
`ibm_fez` backend using 1024 shots.

The hardware experiment produced:

- `00`: 479 measurements
- `11`: 507 measurements
- `01`: 21 measurements
- `10`: 17 measurements

Thus, `00` and `11` accounted for **986 out of 1024 measurements (96.29%)**.

---

### 02. Bloch Sphere and Q-Sphere Visualization

This experiment explores the visualization of single-qubit quantum states using the **Bloch sphere** and **Q-sphere** representations.

Starting from the initial state $|0\rangle$, a sequence of quantum gates is applied to observe how the qubit state changes.

The experiment demonstrates:

- Initial state $|0\rangle$
- Pauli-X gate
- Hadamard gate
- Pauli-Z gate
- Statevector representation
- Bloch sphere visualization
- Q-sphere visualization
- Geometric interpretation of single-qubit states

The sequence demonstrates the transformations:

$$
|0\rangle
\xrightarrow{X}
|1\rangle
\xrightarrow{H}
|-\rangle
\xrightarrow{Z}
|+\rangle
$$

where

$$
|-\rangle =
\frac{|0\rangle - |1\rangle}{\sqrt{2}}
$$

and

$$
|+\rangle =
\frac{|0\rangle + |1\rangle}{\sqrt{2}}.
$$

---

### 03. Quantum Teleportation

This experiment demonstrates the quantum teleportation protocol using Qiskit and real IBM Quantum hardware.

The experiment includes:

- Preparation of an arbitrary quantum state
- Creation of a shared Bell state between Alice and Bob
- Alice's Bell-basis measurement
- Classical communication of Alice's measurement results
- Conditional quantum corrections on Bob's qubit
- Verification of the teleported state
- Execution on a real IBM Quantum processor
- Teleportation after separating the entangled qubits using SWAP operations
- Observation of hardware noise and additional errors introduced by the SWAP operations

The teleportation protocol is based on a shared entangled Bell pair:

$$
|\Phi^+\rangle =
\frac{|00\rangle + |11\rangle}{\sqrt{2}}
$$

Alice's unknown state can be represented as:

$$
|\psi\rangle =
\alpha|0\rangle + \beta|1\rangle
$$

where $\alpha$ and $\beta$ are complex probability amplitudes satisfying:

$$
|\alpha|^2 + |\beta|^2 = 1.
$$

The experiment demonstrates that the quantum state $|\psi\rangle$ can be reconstructed at Bob's qubit using shared entanglement and classical communication, without directly transmitting the physical qubit containing the original state.

---

## Technologies

- Python
- Qiskit
- Qiskit IBM Runtime
- IBM Quantum
- Matplotlib
- JupyterLab
- NumPy

---

## Repository Structure

```text
qiskit-quantum-circuits/
│
├── 01_quantum_entanglement.ipynb
├── 02_bloch_and_q_sphere.ipynb
├── 03_quantum_teleportation.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Future Experiments

Additional quantum-computing experiments will be added to this repository, including:

- Deutsch-Jozsa Algorithm
- Bernstein-Vazirani Algorithm
- Grover's Search Algorithm
- Variational Quantum Algorithms
- Quantum error mitigation experiments
- Quantum error correction experiments

---

## Author

**Sohom Ray Mandal**

B.Tech Electrical Engineering  
Indian Institute of Technology Tirupati

GitHub: [Luzaryal](https://github.com/Luzaryal)