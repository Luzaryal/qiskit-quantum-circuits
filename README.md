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
`ibm_marrakesh` backend using 1024 shots.

The hardware experiment produced:

- `00`: 502 measurements
- `11`: 497 measurements
- `01`: 7 measurements
- `10`: 18 measurements

Thus, `00` and `11` accounted for **999 out of 1024 measurements (97.56%)**.

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
├── 02_Bloch_and_Q_Sphere.ipynb
├── README.md
├── requirements.txt
└── .gitignore