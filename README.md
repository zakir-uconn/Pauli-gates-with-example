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
Input state: \(\ket{0}\)

Apply \(X\):
\[
X\ket{0} = 
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
\begin{bmatrix}
1 \\
0
\end{bmatrix}
=
\begin{bmatrix}
0 \\
1
\end{bmatrix}
= \ket{1}
\]

Result: \(\ket{1}\)

**Geometric Interpretation:**
The \(X\) gate rotates the qubit by 180° around the X-axis on the Bloch sphere.

---

## 2. Pauli-Y Gate (\(Y\))

The \(Y\) gate combines a bit-flip (\(X\)) and a phase-flip (\(Z\)) operation. It is represented as:
\[
Y = iXZ
\]

Matrix form:
\[
Y = 
\begin{bmatrix}
0 & -i \\
i & 0
\end{bmatrix}
\]

### Example:
Input state: \(\ket{0}\)

Apply \(Y\):
\[
Y\ket{0} = 
\begin{bmatrix}
0 & -i \\
i & 0
\end{bmatrix}
\begin{bmatrix}
1 \\
0
\end{bmatrix}
=
\begin{bmatrix}
0 \\
i
\end{bmatrix}
= i\ket{1}
\]

Result: \(i\ket{1}\) (a global phase factor \(i\) is added).

**Geometric Interpretation:**
The \(Y\) gate rotates the qubit by 180° around the Y-axis on the Bloch sphere.

---

## 3. Pauli-Z Gate (\(Z\))

The \(Z\) gate introduces a phase flip. It leaves \(\ket{0}\) unchanged but flips the sign of \(\ket{1}\):

\[
\ket{0} \rightarrow \ket{0}, \quad \ket{1} \rightarrow -\ket{1}
\]

Matrix form:
\[
Z = 
\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
\]

### Example:
Input state: \(\ket{1}\)

Apply \(Z\):
\[
Z\ket{1} = 
\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
\begin{bmatrix}
0 \\
1
\end{bmatrix}
=
\begin{bmatrix}
0 \\
-1
\end{bmatrix}
= -\ket{1}
\]

Result: \(-\ket{1}\)

**Geometric Interpretation:**
The \(Z\) gate rotates the qubit by 180° around the Z-axis on the Bloch sphere.

---

## Comparison of Pauli Gates

| Gate      | Operation                | Matrix                                      | Geometric Effect                   |
|-----------|--------------------------|---------------------------------------------|-------------------------------------|
| Pauli-X   | Bit-flip (NOT gate)      | \(\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}\) | Rotate 180° around X-axis          |
| Pauli-Y   | Bit-flip + Phase-flip    | \(\begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}\) | Rotate 180° around Y-axis          |
| Pauli-Z   | Phase-flip               | \(\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}\) | Rotate 180° around Z-axis          |

---

### How to Use Pauli Gates

Pauli gates are used in:
1. **Quantum Error Correction**: Detect and correct bit-flip and phase-flip errors.
2. **Grover's Algorithm**: Mark and amplify states in a quantum search.
3. **Quantum Chemistry**: Simulate molecular Hamiltonians.

For more details, refer to [Qiskit Documentation](https://qiskit.org/documentation/).
