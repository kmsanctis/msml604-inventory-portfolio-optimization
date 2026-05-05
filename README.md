# Portfolio-Inspired Inventory Optimization
### MSML 604 - Introduction to Optimization | Spring 2026
**Author:** Keegan Sanctis | **UID:** 122067684
**University of Maryland, College Park**

---

## Project Overview

This project adapts the Markowitz mean-variance portfolio optimization framework to the multi-item inventory management problem, applied to a real-world dataset from RoyalTech Electrical & Contracting Co., a retail business in Kuwait specializing in low-to-medium voltage electrical components.

The optimization minimizes total inventory cost - comprising holding costs and expected stockout losses - subject to a capital budget constraint, formulated and solved as a convex optimization problem using CVXPY.

**Key Result:** 22.61% cost reduction over uniform baseline allocation across 3,856 active SKUs.

---

## Repository Structure

- portfolio_inventory_optimization.ipynb — Main project notebook
- sku_optimization_results.csv — SKU-level optimization results
- main_parameters.csv — Main parameter dataframe
- efficient_frontier.png — Efficient frontier plot
- baseline_vs_optimized.png — Baseline vs optimized comparison plot
- README.md — This file

---

## Dependencies

Install CVXPY via:
pip install cvxpy

All other packages (pandas, numpy, matplotlib, scipy, shutil) are available in the standard Google Colab environment.

---

## Data

Since the dataset is proprietary, full end-to-end reproduction requires access to the original data files. The notebook is provided for code review and methodology verification purposes. All outputs, results, and plots are saved in this repository and reflect the actual results produced during execution with the full dataset. Note: For complete reproduction data files can be provided

---

## How to Run

1. Open portfolio_inventory_optimization.ipynb in Google Colab
2. Mount your Google Drive when prompted
3. Update file paths in the Data Loading section (Note: data files can be provided)
4. Run all cells from top to bottom (Runtime → Run all)

---

## Results Summary

Active SKUs: 3,856
Budget (50% level): 66,507 KWD
Full stocking cost: 133,014 KWD
Optimized total cost: 101,144 KWD
Baseline total cost: 130,686 KWD
Cost reduction: 29,542 KWD
Percentage improvement: 22.61%

---

## References

Markowitz, H. (1952). Portfolio selection. The Journal of Finance, 7(1), 77–91.
Arrow, K. J., Harris, T., & Marschak, J. (1951). Optimal inventory policy. Econometrica, 19(3), 250–272.
Diamond, S., & Boyd, S. (2016). CVXPY: A Python-embedded modeling language for convex optimization. JMLR, 17(83), 1–5.
Boyd, S., & Vandenberghe, L. (2004). Convex Optimization. Cambridge University Press.
Nahmias, S., & Olsen, T. L. (2015). Production and operations analysis (7th ed.). Waveland Press.
Silver, E. A., Pyke, D. F., & Thomas, D. J. (2017). Inventory and production management in supply chains (4th ed.). CRC Press.
