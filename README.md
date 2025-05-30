# Forecasting London Logistics Real Estate (LRE) Yields
This repository contains the codebase for a forecasting model designed to predict Net Initial Yields (NIY) in London’s Logistics Real Estate (LRE) market. It was developed as part of an academic project.

**Data Disclaimer**  
This repository includes **only code**. No proprietary or commercial datasets are included or redistributed. All charts, graphs, and correlation matrices derived from such data have been **intentionally removed** to comply with data licensing agreements. Some limited `print()` outputs (e.g., sample values or column names) remain for demonstration purposes and are permitted.
To comply with licensing restrictions:
- **All charts, plots, and graphs** based on proprietary data (e.g., CoStar, CBRE) have been **removed**.
- Code for plotting may remain, but no visual output is rendered or exported.
This has limited the visuals in the Notebook, however is necessary in order to comply with data licensing restrictions. The code still remains. 

## Overview
The goal of this project is to improve NIY forecast accuracy in the logistics sector by combining economic theory with regularised regression techniques for forecasting and prediction. This enables more robust, risk-adjusted decision-making in a volatile market.

## Methodology
The model uses a hybrid econometric and machine learning approach, with a focus on variable selection stability and interpretability:
- **LASSO regression** with 5-fold time-series cross-validation
- **Bootstrapping** (1,000 iterations) for stability validation
- **Feature engineering**: lagged variables, transformations, interaction variables

## Results
- **Performance**:  
  - R² = 0.66  
  - RMSE = 0.37%  
- **Model insights**:  
  - 11 high-confidence predictors identified  
  - Strong influence of microeconomic variables (e.g., Net Absorption, Vacancy Rate)
