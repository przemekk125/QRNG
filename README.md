# Quantum Random Number Generator (QRNG)

## Overview
This project implements a Quantum Random Number Generator (QRNG) using Qiskit, a quantum computing framework. Unlike classical random number generators that rely on algorithms or pseudo-randomness, this QRNG uses the principles of quantum mechanics to produce true randomness.

### Key Features
- Generates quantum-random binary sequences.
- Converts binary sequences into floating-point numbers.
- Demonstrates quantum principles such as superposition through practical implementation.

---

## How It Works
1. **Quantum Bit (Qubit)**:
   Qubits are placed into a state of superposition using the Hadamard gate (H-gate). When measured, each qbit collapses to either `0` or `1` with equal probability, producing randomness.

2. **Binary Sequence Generation**:
   By preparing and measuring multiple qubits, the circuit generates a sequence of random bits.

3. **Random Float Conversion**:
   Binary sequences are interpreted as fractional numbers to produce a floating-point number between `0` and `1`.

---

## Project Requirements
- Python 3.8+
- Qiskit
- Jupyter Notebook

---

## Usage
### Generate n random bits, m times
```python
random_bits = generate_random_bits(m,n)
print("Random Bits:", random_bits)
```

### Generate m random floats, each using n bits
```python
random_float = bits_to_float(generate_random_bits(m,n))
print("Random Float (0 to 1):", random_float)
```
---

## Results
By executing this QRNG, you should observe:
- A list of random floats in the range `[0, 1)` (e.g., `0.7465834309463501`).

---

## References
- [Qiskit Documentation](https://qiskit.org/documentation/)
- [IBM Quantum](https://quantum-computing.ibm.com/)
- [Hadamard Gate](https://en.wikipedia.org/wiki/Hadamard_transform)

---

## License
This project is licensed under the MIT License. Feel free to use, modify, and distribute!


