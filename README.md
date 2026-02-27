# Quantum Computing Assignment 1: Entanglement-Based Quantum Communication

## 📋 Overview

This repository contains solutions to Assignment 1 on **Entanglement-Based Quantum Communication**, covering two fundamental quantum information protocols:
1. **Quantum Teleportation** - Transferring quantum states using entanglement
2. **Superdense Coding** - Sending 2 classical bits using 1 qubit

**Total Marks:** 30 (Problem 1: 15 marks, Problem 2: 10 marks + Conceptual: 5 marks)

## 🎯 Assignment Problems

### Problem 1: Quantum Teleportation (15 Marks)

Implements the quantum teleportation protocol to transfer an arbitrary quantum state from Alice to Bob using:
- Bell pair entanglement
- Bell-basis measurement (without collapse in simulation)
- Quantum correction gates (CX and CZ)
- Verification using inverse unitary transformation

**Key Features:**
- ✅ Arbitrary qubit preparation with Ry(θ) and Rz(φ) rotations
- ✅ Bell state creation: |φ+⟩ = (|00⟩ + |11⟩)/√2
- ✅ Fully quantum correction (no classical bits in simulation)
- ✅ Verification: Bob measures |0⟩ with 100% probability after applying U†

**Results:** Successfully teleports quantum state with 100% fidelity!

### Problem 2: Superdense Coding (10 Marks)

Demonstrates how to send 2 classical bits using only 1 qubit with pre-shared entanglement.

**Encoding Scheme:**
| Message | Gate Applied |
|---------|--------------|
| 00      | I (Identity) |
| 01      | Z            |
| 10      | X            |
| 11      | X then Z     |

**Key Features:**
- ✅ Bell pair distribution
- ✅ Message encoding (chosen message: '10')
- ✅ Bell-basis decoding
- ✅ Comprehensive verification of all 4 possible messages

**Results:** Successfully transmits 2 classical bits with 100% accuracy!

```bash
# Required Python packages
pip install qiskit qiskit-aer numpy matplotlib
