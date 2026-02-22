# MAT1856 / APM466 - Assignment 1

This repository contains the code and report workflow for Assignment 1, focused on:
- Yield-to-maturity (YTM) curve construction
- Spot curve bootstrapping
- 1y-start forward curve construction
- PCA analysis of yield/spot/forward log-returns

## Files

- `Assignment1.ipynb` - main notebook with all calculations, plots, tables, and PCA outputs
- `bond_spec_data.csv` - bond metadata (coupon, face value, maturity, etc.)
- `bond_price_data.csv` - market price observations by bond and date
- `README.md` - this file

## Environment

Use Python 3.10+ and install:

```bash
pip install numpy pandas scipy matplotlib seaborn
```

## How To Run

1. Open `Assignment1.ipynb`.
2. Run cells top-to-bottom.
3. The notebook will:
   - clean and merge bond spec + price data
   - compute accrued interest and dirty prices
   - solve YTM via root finding
   - bootstrap spot rates from dirty prices
   - construct forward rates from interpolated spot curves
   - compute covariance/correlation matrices
   - compute eigenvalues/eigenvectors (principal directions)

## Outputs

The notebook generates:
- YTM, spot, and forward curve plots
- Covariance/correlation heatmaps
- Eigenvalue and principal-direction tables
