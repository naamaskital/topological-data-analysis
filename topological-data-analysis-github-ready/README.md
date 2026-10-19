# Topological Data Analysis — Persistent Homology Experiments

A university course project exploring **persistent homology** and **Vietoris–Rips filtrations** using Python and GUDHI.

**Authors:** Naama Skital and Adir Ofir. This repository contains the computational Part B of a jointly submitted course assignment.

## Highlights

- Reproduce a hand-computed filtered simplicial complex and its H₀/H₁ persistence intervals.
- Generate and analyze four synthetic point clouds: noisy circle, figure-eight, separated circles, and nested circles.
- Plot persistence diagrams and barcodes.
- Compare simplex counts at different maximum edge lengths.
- Test stability under Gaussian perturbations across six noise levels and five random seeds each (30 experiments).
- Calculate bottleneck distances and check the bound `d_B(D_clean, D_noisy) <= 2 * max_point_displacement` for the experiments.

## Technologies

Python · NumPy · Pandas · Matplotlib · GUDHI · Jupyter Notebook

## Run locally

```bash
python -m venv .venv
# macOS / Linux:
source .venv/bin/activate
# Windows PowerShell: .venv\\Scripts\\Activate.ps1
pip install -r requirements.txt
jupyter notebook notebooks/topological_analysis.ipynb
```

Run the notebook cells from top to bottom. The notebook also contains a `%pip install -q gudhi` cell, which is optional after installing requirements.

## Notes

Persistent homology is computed over F₂, and Rips complexes are constructed up to dimension 2. Fixed random seeds are used to make the synthetic experiments reproducible.

The notebook is the original computational submission, with no claims that the underlying GUDHI algorithms were implemented from scratch.

## Publication checklist

- Confirm that publishing the course assignment is permitted.
- Confirm coauthor consent.
- Remove personal ID numbers from any reports or notebooks before publication.
- Verify execution and dependency compatibility in your environment.
