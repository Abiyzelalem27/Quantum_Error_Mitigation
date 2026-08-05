

# QEM – Quantum Error Mitigation

[![Python Version](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-Apache%202.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
[![Qiskit](https://img.shields.io/badge/Qiskit-1.0+-purple.svg)](https://qiskit.org/)

A comprehensive, production-ready Python package for quantum error mitigation techniques, consolidating the methodologies from the Qiskit Global Summer School 2026 Labs 3, 4b, and 4c.

## 📋 Overview

**QEM** provides a unified interface for applying state-of-the-art quantum error mitigation techniques, including:

- **Samplomatic & Advanced Mitigation** – Boxing, Twirling, NoiseLearnerV3, Propagated Noise Absorption (PNA), and Shaded Lightcones (SLC)
- **QAOA for Partition Problems** – Graph mapping, Quantum Approximate Optimization Algorithm, Pauli Correlation Encoding, and multiple error mitigation strategies (M3, ZNE, PEC)
- **Sample-based Quantum Diagonalization** – Molecular ground-state estimation for N₂ using SQD with LUCJ ansatz

All techniques are implemented in a modular, well-tested, and production-ready format suitable for research and industrial applications.

## 🚀 Features

- **Modular Architecture**: Clean separation of concerns with dedicated subpackages for each lab.
- **Hardware-Ready**: Seamless integration with Qiskit Runtime for execution on IBM Quantum hardware.
- **Comprehensive Error Mitigation**: Support for TREX, ZNE, PEC, M3, Dynamical Decoupling, and Pauli Twirling.
- **Scalable**: Pauli Correlation Encoding reduces qubit requirements for large problems.
- **Reproducible**: Fixed seeds, job ID management, and pre-trained parameters included.
- **Well-Tested**: Unit tests and continuous integration ready.

## 📦 Installation

### From PyPI (coming soon)

```bash
pip install qem

# Clone the repository
git clone https://github.com/Abiyzelalem27/quantum-error-mitigation.git
cd quantum-error-mitigation

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install in development mode
pip install -e .

# Or install with development dependencies
pip install -e ".[dev]"

from qem import (
    # Lab 3: Samplomatic & Advanced Mitigation
    construct_ising_circuit,
    generate_noise_mitigating_observable,
    compute_local_scales,
    
    # Lab 4b: QAOA & Partition Problem
    build_partition_graph,
    configure_estimator_options,
    reduce_qubits_with_pce,
    
    # Lab 4c: Sample-based Quantum Diagonalization
    build_n2_molecule,
    run_sqd_loop,
    
    # Utilities
    get_backend,
    plot_partition_graph,
)

# Example: Build a partition graph
numbers = [3, 5, 7, 9, 11, 13]
graph = build_partition_graph(numbers)

# Example: Configure error mitigation
options = configure_estimator_options(method='zne', shots=2000)

# Example: Get a backend
backend = get_backend(family='Heron')

qem/
├── notebooks/                          
│   ├── 01_samplomatic_advanced_mitigation/  
│   ├── 02_qaoa_partition_problem/          
│   └── 03_sample_based_quantum_diagonalization/ 
├── src/
│   └── qem/                             
│       ├── qaoa_partition_problem/      
│       ├── sample_based_quantum_diagonalization/ 
│       ├── samplomatic_advanced_mitigation/ # Samplomatic (Lab 3)
│       └── utils/                       # Shared utilities
├── tests/                              # Unit tests
├── data/                               # Pre-trained parameters
├── pyproject.toml                      # Package metadata
├── requirements.txt                    # Core dependencies
└── README.md                           # This file

