# Quantum Supply Chain Routing
# Quantum-Enhanced Supply Chain Routing (VRP)
**Qiskit Fall Fest 2026 — Florida Institute of Technology**  
**Author:** Ayodeji Williams (M.S. Operations Research)

---

## Overview
As part of the **Florida Qiskit Fallfest Hackathon** celebrating a decade of quantum on the cloud, this project addresses a classic **Vehicle Routing Problem (VRP)**. Leveraging an Operations Research background, this project models multi-vehicle logistics constraints, maps them into a Quadratic Unconstrained Binary Optimization (QUBO) formulation, and solves them using Qiskit.

## Project Structure
* **Problem Definition:** Formulating a multi-vehicle routing problem with a central depot and customer nodes under spatial and fleet constraints.
* **QUBO & Optimization:** Translating combinatorial routing constraints into quadratic programs using `qiskit-optimization`.
* **Validation & Benchmarking:** Comparing quantum-ready problem formulations against exact classical solvers (`NumPyMinimumEigensolver`).
* **Route Visualization:** Clean Matplotlib/NetworkX mapping displaying optimized paths for delivery fleets.

## Results Summary
| Metric | Classical Baseline (Exact) | Quantum-Enhanced (QUBO / Model) |
| :--- | :--- | :--- |
| **Optimization Approach** | Exact Solver | Hybrid QUBO Mapping |
| **Total Route Distance** | 18.61 units | Optimal Match |
| **Fleet Utilization** | 2 Vehicles | 2 Vehicles |
| **Constraint Satisfaction**| 100% Valid | 100% Valid (Penalty Tuned) |

## How to Run
1. Clone this repository.
2. Open the `Quantum.ipynb` Jupyter Notebook in Google Colab or a local environment.
3. Ensure required dependencies are installed:
   ```bash
   pip install qiskit qiskit-ibm-runtime qiskit-optimization networkx matplotlib pandas
