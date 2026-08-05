

# Quantum Error Mitigation

[![Python 3.11+](https://img.shields.io/badge/python-3.11%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Project Status](https://img.shields.io/badge/status-research%20and%20learning-orange.svg)](#project-status)

A modular research and learning repository for studying **quantum error mitigation, noise-aware quantum algorithms, and hybrid quantum–classical methods**.
The project focuses on understanding how noise affects quantum computations and how mitigation techniques can improve the quality of measured results.

---

## objectives


- quantum noise and its effect on circuit results;
- error suppression and error mitigation methods;
- noise-aware execution of quantum algorithms;
- comparison of mitigated and unmitigated results;
- hybrid quantum–classical optimization;
- scalable methods for quantum simulation and optimization;
- reusable Python tools for quantum-error-mitigation studies.

---

## Main topics

### Quantum Approximate Optimization Algorithm

The QAOA notebooks study the number-partition problem, including:

- problem formulation;
- graph and Hamiltonian construction;
- QAOA circuit design;
- parameter optimization;
- noise analysis;
- error-mitigation comparisons;
- scaling with Pauli Correlation Encoding.

### Sample-Based Quantum Diagonalization

The SQD notebooks explore hybrid quantum–classical estimation of molecular ground-state energies through:

- quantum-state preparation;
- sampling of electron configurations;
- configuration recovery;
- reduced-subspace construction;
- classical diagonalization;
- comparison with classical reference methods.

### Advanced quantum error mitigation

The advanced-mitigation notebooks investigate:

- Pauli twirling;
- circuit boxing;
- layerwise noise learning;
- mirror circuits;
- propagated noise absorption;
- readout-error mitigation;
- probabilistic error cancellation;
- mitigation bias and sampling cost.

---

## Repository structure

```text
Quantum_Error_Mitigation/
├── notebooks/
│   ├── qaoa_partition_problem/
│   │   ├── qaoa_theory_setup.ipynb
│   │   ├── qaoa_error_mitigation.ipynb
│   │   └── qaoa_scaling_pce.ipynb
│   │
│   ├── sample_based_quantum_diagonalization/
│   │   ├── sqd_setup_ansatz.ipynb
│   │   └── sqd_sampling_diagonalization.ipynb
│   │
│   └── samplomatic_advanced_mitigation/
│       ├── theory_estimator.ipynb
│       ├── boxing_twirling.ipynb
│       ├── noise_learning_executor.ipynb
│       ├── Ising_chain_Mirror_trick.ipynb
│       └── PNA_TREX_comparison.ipynb
│
├── src/
│   └── qem/
│       ├── qaoa_partition_problem/
│       ├── sample_based_quantum_diagonalization/
│       ├── samplomatic_advanced_mitigation/
│       └── utils/
│
├── tests/
├── pyproject.toml
├── requirements.txt
├── requirements-dev.txt
├── LICENSE
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Abiyzelalem27/Quantum_Error_Mitigation.git
cd Quantum_Error_Mitigation
```


---

## Repository

```text
Quantum Error Mitigation
https://github.com/Abiyzelalem27/Quantum_Error_Mitigation
```
