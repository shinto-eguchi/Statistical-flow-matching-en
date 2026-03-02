[README.md](https://github.com/user-attachments/files/25674773/README.md)
# Flow Matching / Statistical Demos (Jupyter notebooks)

This repository collects minimal demo notebooks that use generative models (mainly Flow Matching)
as **extensions and calibrators of statistical models**.
To make the notebooks readable directly on GitHub, each notebook starts with a short overview.

## Included notebooks

- `SM-ML_GMM1.ipynb`: Comparison of Penalized MLE and Penalized Score Matching for a Gaussian Graphical Model (GGM)
- `FM_Copula1.ipynb`: A demo of learning a copula (S-shaped dependence) via Flow Matching
- `OT_Coupling1.ipynb`: Flow Matching with mini-batch Optimal Transport (Hungarian) coupling (two-moons)
- `MI-FM1.ipynb`: A minimal demo of Multiple Imputation using Flow Matching (as a basis for comparison with IterativeImputer)
- `RF_FM1.ipynb`: Estimating interventional distributions p(y | do(A=a))
  (RF mean + scale + residual resampling vs Flow Matching)
- `Cox_FM_PH_model1.ipynb`: Cox PH diagnostics and calibration by Cox + Flow(tt) (calls R via rpy2)

> Execution steps, I/O, and notes are summarized in the “Overview” cell at the top of each notebook.

## Quickstart (Python)

### 1) Create a virtual environment (recommended)
```bash
python -m venv .venv
# Windows (PowerShell)
.venv\Scripts\Activate.ps1
# macOS/Linux
source .venv/bin/activate
