# Time Series Analysis with VECM-GARCH on streamlit

## Overview

This Streamlit application provides a comprehensive framework for multivariate time series analysis using Vector Error Correction Models (VECM) and Generalized Autoregressive Conditional Heteroskedasticity (GARCH) modeling. It's designed for economists, financial analysts, and researchers working with cointegrated time series data.

## Features

- **Data Processing**: Upload and preprocess time series data with automatic frequency detection
- **Stationarity Testing**: Augmented Dickey-Fuller tests with automatic differencing
- **Lag Selection**: Information criteria-based optimal lag selection (AIC, BIC, FPE, HQIC)
- **Cointegration Analysis**: Johansen tests for detecting long-run relationships
- **VECM Estimation**: Full model estimation with customizable deterministic terms
- **Impulse Response Analysis**: Dynamic response visualization with confidence intervals
- **Residual Diagnostics**: Comprehensive tests for model validation
- **GARCH Modeling**: Volatility analysis with multiple GARCH specifications
- **Visualization**: Interactive plots for all analysis components
- **Result Export**: Download detailed analysis results in ZIP format

## How It Works

1. **Upload Data**: CSV or Excel files with time series data
2. **Configure Analysis**: Set parameters for VECM and GARCH modeling
3. **Run Analysis**: Automated pipeline performs all analytical steps
4. **Interpret Results**: View detailed outputs and visualizations
5. **Export Findings**: Download comprehensive reports and figures

## Methodology

The application implements a rigorous statistical workflow:

1. **Data Validation**: Checks for time series properties and stationarity
2. **Cointegration Testing**: Identifies long-run equilibrium relationships
3. **VECM Specification**: Estimates adjustment mechanisms and short-run dynamics
4. **Impulse Response Analysis**: Examines system responses to shocks
5. **Residual Diagnostics**: Validates model assumptions
6. **GARCH Modeling**: Captures conditional heteroskedasticity in residuals

## Usage Requirements

- Time series data with at least 2 variables
- Recommended minimum of 100 observations
- Data should be potentially cointegrated (integrated of the same order)
- CSV or Excel format with a date/time index column

## Installation

```bash
# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run vecmgarch.py
```
