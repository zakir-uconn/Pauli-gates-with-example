# Pauli-gates-with-example

Pauli gates are fundamental single-qubit quantum gates associated with the Pauli matrices. They represent basic quantum operations in quantum computing. The three types of Pauli gates are:

- **Pauli-X gate (X)**
- **Pauli-Y gate (Y)**
- **Pauli-Z gate (Z)**

Each Pauli gate corresponds to a specific operation on the Bloch sphere. Below are their mathematical definitions and examples.

---

## 1. Pauli-X Gate (X)
<img width="463" alt="image" src="https://github.com/user-attachments/assets/4b0272d1-b7e4-460a-a403-598e90a379ce">


### Example:
<img width="289" alt="image" src="https://github.com/user-attachments/assets/d72ccf4c-f4b9-4b94-b29e-6fc007823c4c" />

**Geometric Interpretation:**
The \(X\) gate rotates the qubit by 180° around the X-axis on the Bloch sphere.

---

## 2. Pauli-Y Gate \(Y\)
<img width="350" alt="image" src="https://github.com/user-attachments/assets/a842ad74-1bfb-4098-a2e7-2dc29bf7be4f" />

**Geometric Interpretation:**
The \(Y\) gate rotates the qubit by 180° around the Y-axis on the Bloch sphere.

---

## 3. Pauli-Z Gate \(Z\)
<img width="314" alt="image" src="https://github.com/user-attachments/assets/0951e05f-910e-4316-8a3e-29ca06061911" />


**Geometric Interpretation:**
The \(Z\) gate rotates the qubit by 180° around the Z-axis on the Bloch sphere.

---

## Comparison of Pauli Gates

| Gate      | Operation                | Matrix                                      | Geometric Effect                   |
|-----------|--------------------------|---------------------------------------------|-------------------------------------|
| Pauli-X   | Bit-flip (NOT gate)      | <img width="31" alt="image" src="https://github.com/user-attachments/assets/aeded10c-2096-4207-a0e2-27f7273f7a87" />| Rotate 180° around X-axis          |
| Pauli-Y   | Bit-flip + Phase-flip    | <img width="35" alt="image" src="https://github.com/user-attachments/assets/c10a497f-88b2-4bb3-b890-075bdd534e6c" />| Rotate 180° around Y-axis          |
| Pauli-Z   | Phase-flip               | <img width="33" alt="image" src="https://github.com/user-attachments/assets/b66dd3a7-b29d-499c-a5b6-20bf414535cc" />| Rotate 180° around Z-axis          |

---

### How to Use Pauli Gates

Pauli gates are used in:
1. **Quantum Error Correction**: Detect and correct bit-flip and phase-flip errors.
2. **Grover's Algorithm**: Mark and amplify states in a quantum search.
3. **Quantum Chemistry**: Simulate molecular Hamiltonians.

For more details, refer to [Qiskit Documentation](https://qiskit.org/documentation/).
