This repository contains all data processing, econometric estimation, and replication code for:

**Venkateswaran, C. (2026).  
“Inflation Surprises and Municipal Bond Pricing: Evidence from Green and Conventional Municipal Bond Indices.”**

# Overview

The project studies whether U.S. green municipal bonds differ from conventional municipal bonds in their exposure to inflation surprises. Using monthly data (2016–2025), it estimates local-projection impulse responses of green–minus–vanilla municipal bond return spreads to inflation forecast errors constructed from CPI inflation and University of Michigan inflation expectations.

The analysis includes:

- Frequentist local projections with HAC inference  
- Bayesian ridge-regularized local projections  
- Cumulative impulse responses  
- Discount-rate mediation tests using Treasury yield controls  
- Placebo and robustness checks (lag length, HAC bandwidth)

# Repository Structure

| File | Description |
|
| `Venkateswaran_TermPaper_MunicipalBonds.pdf` | Main paper |
| `Venkateswaran_TermPaper_Mathematical_Appendix.pdf` | Estimation derivations and Bayesian details |
| `Venkateswaran_TermPaper_Appendix.pdf` | Robustness and falsification tests |
| `Venkateswaran_TermPaper_PythonCode.pdf` | Full replication code |
| `FREDCPIAUCSL.csv` | CPI data (FRED) |
| `MICH.csv` | Michigan inflation expectations (FRED) |
| `DGS10.csv` | 10-year Treasury yield (FRED) |
| `SP500MUNIBOND.xls` | S&P Municipal Bond Index |
| `SP5500GREENBOND.xls` | S&P Municipal Green Bond Index |

# Requirements

Python 3.9+ with:

- numpy  
- pandas  
- matplotlib  
- scipy  
- statsmodels  

# Replication

1. Place all CSV/XLS data files in the project root.
2. Run the Python code in `Venkateswaran_TermPaper_PythonCode.pdf` (or copy into a `.py`/`.ipynb` file).
3. All figures and tables from the paper will be reproduced automatically.
