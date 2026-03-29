# Forecasting Monthly Beer Production in Australia: A Comparative Time Series Analysis

## What the Project Does

This project **compares three time series forecasting models** (ARIMA, SARIMA, and Facebook Prophet) to predict monthly beer production in Australia from 1956 to 1995.

### Key Activities:

1. **Analyzes historical data** (476 months) to identify patterns:
   - Strong seasonal cycles (peak in December, low in June)
   - Long-term trend (growth until 1980s, then decline)

2. **Builds and evaluates three forecasting models**:
   - **ARIMA(4,1,2)**: Baseline model, MAPE = 10.10%
   - **SARIMA(2,1,2)(0,1,1)**: Seasonal model, MAPE = 6.13% (best accuracy)
   - **Prophet**: Automated model, MAPE = 6.33% (most interpretable)

3. **Generates 24-month forecasts** and visualizes results with confidence intervals

4. **Provides insights** for production planning and inventory management

### Output:
- 10+ visualizations (time series, decomposition, forecasts)
- Model performance comparison tables
- Cleaned dataset and forecast results (CSV files)
- Summary reports
---

## Execution Guide

Run the cells in order.

---
## Library Versions

| Package | Version |
|---------|---------|
| Python | 3.12.13 |
| pandas | 2.2.2 |
| numpy | 2.0.2 |
| matplotlib | 3.10.0 |
| seaborn | 0.13.2 |
| statsmodels | 0.14.6 |
| scikit-learn | 1.6.1 |
| scipy | 1.16.3 |
| prophet | 1.3.0 |

---

## Repository Structure
```
beer-production-analysis/
│
├── data/
│   └── monthly-beer-production-in-austr.csv
│
├── notebooks/
│   └── COMP5152_Group45.ipynb
│
├── outputs/
│   ├── plots/
│   │   ├── 01_main_time_series.png              # DATA LOADING AND PREPROCESSING
│   │   ├── 02_production_distribution.png       # DATA LOADING AND PREPROCESSING
│   │   ├── 03_production_by_decade.png          # DATA LOADING AND PREPROCESSING
│   │   ├── 04_monthly_production_pattern.png    # DATA LOADING AND PREPROCESSING
│   │   ├── 05_recent_years_comparison.png       # DATA LOADING AND PREPROCESSING
│   │   ├── 06_trend_component.png               # DATA LOADING AND PREPROCESSING
│   │   ├── 07_seasonal_component.png            # DATA LOADING AND PREPROCESSING
│   │   ├── 08_residual_component.png            # DATA LOADING AND PREPROCESSING
│   │   ├── 09_seasonal_decomposition_summary.png # DATA LOADING AND PREPROCESSING
│   │   ├── 10_residual_analysis.png             # DATA LOADING AND PREPROCESSING
│   │   ├── 02_acf_pacf_analysis.png             # ARIMA
│   │   ├── 04_model_diagnostics.png             # ARIMA
│   │   ├── 05_final_forecast.png                # ARIMA
│   │   ├── 09_final_sarima_forecast.png         # SARIMA
│   │   └── 10_prophet_analysis.png              # Prophet
│   │
│   ├── csv/
│   │   ├── monthly-beer-production-cleaned.csv  # DATA LOADING AND PREPROCESSING
│   │   ├── 06_future_forecast.csv               # ARIMA
│   │   ├── 09_sarima_test_predictions.csv       # SARIMA
│   │   ├── 09_sarima_future_forecast.csv        # SARIMA
│   │   ├── 10_prophet_test_predictions.csv      # Prophet
│   │   └── 10_prophet_future_forecast.csv       # Prophet
│   │
│   └── txt/
│       ├── 03_model_summary.txt                 # ARIMA
│       ├── 07_model_summary_report.txt          # ARIMA
│       ├── 09_sarima_summary_report.txt         # SARIMA
│       └── 10_prophet_summary_report.txt        # Prophet


```
