\# Qiskit Quantum Circuits



Quantum computing experiments and implementations using \*\*Qiskit\*\* and \*\*IBM Quantum\*\* hardware.



\## Projects



\### 01. Quantum Entanglement — Bell State



This experiment demonstrates the preparation and measurement of a two-qubit Bell state using Qiskit.



The experiment includes:



\- Construction of the Bell state

&#x20; \\\[

&#x20; |\\Phi^+\\rangle = \\frac{|00\\rangle + |11\\rangle}{\\sqrt{2}}

&#x20; \\]

\- Statevector simulation and theoretical probability analysis

\- 1024-shot ideal simulation

\- Hardware-specific circuit transpilation

\- Execution on a real IBM Quantum processor

\- Comparison between ideal simulation and real hardware results

\- Analysis of hardware noise and measurement errors



The Bell-state circuit was executed on the IBM Quantum `ibm\_marrakesh` backend using 1024 shots.



\## Technologies



\- Python

\- Qiskit

\- Qiskit IBM Runtime

\- IBM Quantum

\- Matplotlib

\- JupyterLab



\## Repository Structure



```text

qiskit-quantum-circuits/

├── 01\_quantum\_entanglement.ipynb

├── requirements.txt

├── README.md

└── .gitignore

