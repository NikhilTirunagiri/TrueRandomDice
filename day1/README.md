# True Random Dice

A quantum computing experiment that uses Qiskit to create a truly random dice roll.

## What it does

This project implements a 6-sided die using quantum mechanics. Instead of relying on pseudo-random number generators, it uses quantum superposition to generate genuinely random outcomes.

## How it works

The quantum dice uses 3 qubits in superposition to generate 8 possible outcomes (0-7). Since we need values 1-6 for a standard die, the function maps outcomes 0-5 to dice values 1-6, and re-rolls if it gets 6 or 7.

## Requirements

- Python 3.x
- Qiskit
- Qiskit Aer (simulator)
- Qiskit IBM Runtime

Install dependencies:
```bash
pip install qiskit qiskit-ibm-runtime qiskit-aer
```

## Usage

Open the Jupyter notebook `TrueRandomDice.ipynb` and run the cells. The main function `roll_the_Qdice()` returns a random number between 1 and 6.

## Why quantum?

Traditional computers use deterministic algorithms to simulate randomness. Quantum mechanics, however, is fundamentally probabilistic. When a qubit in superposition is measured, the outcome is truly random - not just unpredictable to us, but genuinely random according to our best understanding of physics.

Perfect for settling disputes or making important life decisions with maximum cosmic fairness.
