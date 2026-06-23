# Simple Linear Regression – Marketing ROI Analysis

## Project Overview

This project analyzes a marketing dataset to determine which advertising channel — **TV**, **Radio**, or **Social Media** — has the strongest relationship with **Sales**. Using Python and `statsmodels`, a Simple Linear Regression model is built, validated, and interpreted to provide a data-driven recommendation for marketing budget allocation.

## Objective

- Load and clean the marketing dataset
- Perform exploratory data analysis (EDA) to identify the variable most correlated with Sales
- Build and validate an Ordinary Least Squares (OLS) regression model
- Test key regression assumptions (Linearity, Normality, Homoscedasticity, Independence)
- Translate statistical results into a clear, ROI-based business recommendation

## Key Findings

- **TV** advertising spend has a near-perfect correlation with Sales (**r ≈ 0.9995**)
- The OLS model explains approximately **99.9% of the variance** in Sales (**R² ≈ 0.999**)
- The relationship is statistically significant (**p < 0.001**)
- **Recommendation:** Allocate the largest share of the marketing budget to TV advertising, with Radio as a secondary channel.

## Repository Contents

| File                                       | Description                                                                                    |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| `regression_analysis.ipynb`                | Jupyter Notebook with full analysis — EDA, OLS model, diagnostics, and business interpretation |
| `marketing_and_sales_data_evaluate_ir.csv` | Dataset used for the analysis                                                                  |
| `README.md`                                | Project overview and setup instructions                                                        |

## Environment Setup

This project requires Python 3.8+ and the following libraries:

```bash
pip install pandas numpy matplotlib seaborn statsmodels scipy
```

## How to Run

1. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd <repo-folder>
   ```
2. Install the required dependencies (see above)
3. Ensure `marketing_and_sales_data_evaluate_ir.csv` is in the same directory as the notebook
4. Open `regression_analysis.ipynb` in Jupyter Notebook, JupyterLab, or VS Code
5. Run all cells in order (Run All)

## Methodology Summary

1. **Data Cleaning** – Removed rows with missing values (< 0.3% of the dataset)
2. **EDA** – Generated a correlation heatmap and scatter plots for TV, Radio, and Social Media against Sales
3. **Model Building** – Fit an OLS regression model using TV spend as the independent variable
4. **Model Validation** – Verified assumptions using residual plots, a Q-Q plot, and a scale-location plot
5. **Business Interpretation** – Converted statistical output (R², coefficients, p-values) into a marketing budget recommendation

## Author

Happy Oluwafemi Odole
