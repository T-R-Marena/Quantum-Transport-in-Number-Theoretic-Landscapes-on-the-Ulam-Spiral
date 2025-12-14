# Quantum Transport in Number-Theoretic Landscapes on the Ulam Spiral

Google Colab implementation of the paper **"Distinct Universality Classes of Quantum Transport in Number-Theoretic Landscapes on the Ulam Spiral"** by Tommaso R. Marena.

This notebook simulates single-particle quantum wavepacket dynamics on 2D tight-binding lattices where the potential $V(x,y)$ is determined by arithmetic functions (Primes, Möbius, Liouville) embedded on the Ulam spiral.

Google Colab Notebook Link: https://colab.research.google.com/drive/1bvyR4zsQGnJ3AQDUUutD0nSb1xoYUyx2?usp=sharing

GitHub Repository Link: https://github.com/T-R-Marena/Quantum-Transport-in-Number-Theoretic-Landscapes-on-the-Ulam-Spiral

## Quick Start (Google Colab)

### Option 1: Run Directly in Colab (Recommended)
1. Click the "Open In Colab" badge above.
2. Once open, click **"Runtime"** → **"Run all"**.
3. Wait ~5–10 minutes for simulations to complete.

### Option 2: Upload & Run Locally
1. Download the `.ipynb` file.
2. Install dependencies: `pip install -r requirements.txt`
3. Open in Jupyter Notebook and run all cells.

## What's Included

**`Tommaso_R_Marena_Quantum_Transport_in_Number_Theoretic_Landscapes_on_the_Ulam_Spiral.ipynb`**

A single, self-contained Jupyter notebook that includes:
- Number-theoretic function implementations (primes, Möbius, Liouville)
- Ulam spiral geometry construction
- Hamiltonian building and sparse matrix operations
- Time-evolution via `scipy.sparse.linalg.expm_multiply`
- Observable computations (mean-squared radius, participation ratio)
- Power-law exponent fitting (log-log regression)
- Full parameter scan and ensemble averaging
- Figure generation (MSR curves, PR curves, boxplots, heatmaps)

## Key Results

Our simulations demonstrate two distinct universality classes of quantum transport:

1. **Localized Class** ($\alpha_{\mathrm{PR}} \approx 0.1 \pm 0.02$): Prime-number potentials and random (Cramér) controls.
2. **Delocalized Class** ($\alpha_{\mathrm{PR}} \approx 0.6 \pm 0.05$): Multiplicative arithmetic functions (Möbius and Liouville).

This five-fold difference in participation ratio exponent indicates that multiplicative structure drives delocalization, distinct from prime-based or random disorder.

## System Requirements

**Google Colab:** No setup required. All dependencies (NumPy, SciPy, Matplotlib) are pre-installed.

**Local Execution:** Python 3.8+ with the packages listed in `requirements.txt`.

## Outputs

The notebook generates and saves:
- **`figures/fig_msr_curves.pdf`** — Mean-squared radius vs. time
- **`figures/fig_pr_curves.pdf`** — Participation ratio vs. time
- **`figures/fig_exponent_boxplots.pdf`** — Distribution of effective exponents
- **`figures/fig_exponents_pr_heatmap.pdf`** — Parameter robustness heatmap
- **`scan_results/*.npz`** — Raw simulation data

## Citation

If you use this code, please cite the arXiv preprint (currently awaiting approval:

@article{marena2025quantum,
title={Distinct Universality Classes of Quantum Transport in Number-Theoretic Landscapes on the Ulam Spiral},
author={Marena, Tommaso R},
journal={arXiv preprint arXiv:25XX.XXXXX},
year={2025}
}

## License

MIT License. Free to use and modify.
