# Yield Curve Analysis for Canada
## Introduction
A yield curve is a graphical representation of interest rates on debts for a range of maturities. It shows the relationship between the interest rate (or cost of borrowing) and the time to maturity of the debt for a given borrower in a given currency. The curve is often used as a benchmark for other interest rates and as an indicator of economic conditions.

## Contribution
This repository provides tools to analyze and visualize the yield curve for Canada. The main contributions include:
- <b>Yield Curve at a Given Date:</b> Visualize the yield curve observed at a specific date.
- <b>3D Yield Curve:</b> Generate a 3D plot of the yield curve over time.
- <b>Principal Component Analysis (PCA):</b> Perform PCA on the yield curve data to identify the main components driving the changes in the yield curve over time.

For this analysis, I used various Canadian government bond spot rates from 0.25 years up to 10 years to maturity (provided by the Bank of Canada), to see if we can model the yield curve and its slope. When finding the principal components of the yield curve, the main theory held by econometricians is that:

```math
PC1 = constant ≈ long term interest rate ≈ R*
PC2 = slope ≈ term premium
PC3 = curvature
```

## Required Packages
The following packages are required to run the code in this repository:
- numpy
- pandas
- matplotlib
- scikit-learn
