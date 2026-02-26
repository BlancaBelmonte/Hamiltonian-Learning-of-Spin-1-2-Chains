# Hamiltonian Learning of Spin‑1/2 Chains

Quantum Machine Learning assignment  
February 2026

This repository contains the work for a Master’s‑level assignment on
learning Hamiltonians of one‑dimensional spin‑1/2 systems using
classical and quantum‑inspired machine‑learning techniques.

---

## Repository structure

- `simple_limpio.ipynb`  
  A jupyter notebook that creates a dataset, a simple Hamiltonian, a Vanilla Training model and a NDE model and a comparison between them.

- `complejo.ipynb`  
  First exploratory notebook. It walks through generating synthetic
  measurement data, defining a simple spin‑1/2 Hamiltonian, and
  training basic regression models. 

- `complejo_4_model_mismatch.ipynb`  
  Builds on the earlier `complejo.ipynb` experiments but deliberately
  introduces a model mismatch between the Hamiltonian used to
  generate the synthetic data and the one assumed by the learning
  algorithm.  The notebook systematically varies the mismatch and
  evaluates how the estimation error, convergence and generalization
  degrade compared with the matched‑model case.  This helps quantify
  the robustness of different regression approaches under incorrect
  model assumptions.

- `complejo_5_reducir_dataset_robusness.ipynb`  
  A focused study of the robustness of the Hamiltonian‑learning
  procedure. It examines how well the estimated parameters hold up
  under various data‑reduction scenarios and noisy measurements.


## Requirements

- Python 3.8+ (a virtual environment is strongly recommended)
- `numpy`, `scipy`, `matplotlib`, `pandas`
- `qiskit` (if you plan to reproduce quantum‑circuit simulations)

Install dependencies with:

```bash
python -m venv venv
.\venv\Scripts\activate      # Windows
pip install -r requirements.txt 


