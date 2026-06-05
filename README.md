# Cubic Polynomial Fit Research Demo

This Python repo demonstrates how to approximate an irregular nonlinear curve using a **3rd-order polynomial fit**.

It generates:

- Original nonlinear curve data
- Cubic polynomial fitted curve
- Detailed results table as CSV
- Error/residual table
- RMSE, MAE, and R² metrics
- Curve vs fitted curve graph
- Residual error graph
- PDF research-style report with real textbook references

## Mathematical Model

Original nonlinear curve:

```text
y = sin(x) + 0.1x^2 + 0.25sin(2.5x)
```

Cubic fitted model:

```text
y_hat = a3*x^3 + a2*x^2 + a1*x + a0
```

The coefficients are estimated using least-squares polynomial regression.

## Folder Structure

```text
cubic_polyfit_repo/
├── README.md
├── requirements.txt
├── src/
│   └── cubic_fit.py
└── outputs/
    ├── detailed_results.csv
    ├── metrics.csv
    ├── curve_vs_fit.png
    ├── residual_plot.png
    └── cubic_fit_report.pdf
```

## Installation

Create a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run

```bash
python src/cubic_fit.py
```

## Outputs

After running, check the `outputs/` folder.

Main files:

```text
outputs/detailed_results.csv
outputs/metrics.csv
outputs/curve_vs_fit.png
outputs/residual_plot.png
outputs/cubic_fit_report.pdf
```

## References

1. Montgomery, D. C., Peck, E. A., & Vining, G. G. (2021). *Introduction to Linear Regression Analysis*. Wiley.
2. Hastie, T., Tibshirani, R., & Friedman, J. (2009). *The Elements of Statistical Learning*. Springer.
3. Press, W. H., Teukolsky, S. A., Vetterling, W. T., & Flannery, B. P. (2007). *Numerical Recipes: The Art of Scientific Computing*. Cambridge University Press.
