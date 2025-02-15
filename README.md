# Quantum Random OTP Generator

This project implements a Quantum Random Number Generator (QRNG) using Google's Cirq library to generate a One-Time Password (OTP). The randomness is derived from quantum superposition, making it more secure than classical pseudo-random number generators.

## Features
- Utilizes quantum superposition to generate truly random bits
- Converts binary quantum-generated numbers into a numerical OTP
- Customizable OTP length

## Prerequisites
Ensure you have the following dependencies installed:

```sh
pip install cirq numpy
```

## How It Works
1. **Quantum Random Number Generation**:
   - A quantum circuit is created with Hadamard gates to generate random bits.
   - Measurement collapses the qubits into classical random bits.
2. **OTP Generation**:
   - The quantum-generated binary string is converted into a decimal number.
   - The OTP is truncated to the required length.
