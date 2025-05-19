# Hybrid Forecasting for Renewable Energy Market Dynamics

This project focuses on forecasting renewable energy production and market prices using a hybrid machine learning approach. The goal is to enhance grid stability and support informed market decisions in volatile energy environments.

## 🌟 Project Highlights

- **Hybrid Model**: Combines tree-based ML (Random Forest) and time series analysis.
- **Feature Engineering**: Includes lag features, rolling and expanding means.
- **Explainable AI**: SHAP values used for model interpretability.
- **Data**: 58,000+ records (2020–2024), 30-minute intervals of energy and market data.
- **Best Performance**: RF with engineered features (RMSE: 7.24).

## 📊 Key Features

- **Models Used**: 
  - Vector Autoregression (VAR) - baseline
  - Random Forest Regressor - main model
- **Evaluation Metrics**: RMSE, MAE, MSE
- **Top Predictors**: Previous day's price (lag_1), Market Index Price (mip)

## 📁 Project Structure

- `data/`: Contains preprocessed datasets.
- `notebooks/`: Jupyter notebooks for EDA, modeling, and SHAP analysis.
- `models/`: Trained model outputs.
- `visualizations/`: Time series plots, SHAP plots.

## ⚙️ Tools & Libraries

- Python 3.8
- pandas, numpy
- scikit-learn, statsmodels
- matplotlib, seaborn, plotly
- shap

## 🔍 Insights

- Short-term market indicators (like lagged prices) are more predictive than real-time supply.
- Lack of seasonality supports the use of non-linear models.
- SHAP improves trust by explaining model decisions.

## 🔮 Future Directions

- Integrate external data (e.g., weather).
- Expand to other ML models (LSTM, hybrid networks).
- Build real-time updating system for market applications.

