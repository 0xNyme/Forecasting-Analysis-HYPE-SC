# Cryptocurrency Price Forecasting with LSTM
Abstract
This project implements Long Short-Term Memory (LSTM) neural networks and leverages pretrained models to forecast cryptocurrency prices for Hyperliquid (HYPE) and Siacoin (SIA). Using historical price data spanning May 2024 to May 2025, we developed and fine-tuned predictive models that analyze price patterns and generate future price forecasts with confidence intervals.
Key Findings:

- [HYPE](https://github.com/0xNyme/Forecasting-Analysis-HYPE-SC/blob/main/HYPE.md): Combined LSTM and pretrained model predictions show consolidation around $30-35 range after recent rally, with high volatility expected
- [SIA](https://github.com/0xNyme/Forecasting-Analysis-HYPE-SC/blob/main/SC.md): Ensemble approach indicates gradual recovery potential from current oversold levels ($0.003) to $0.004 range

Pretrained models enhanced prediction accuracy and provided additional validation for custom LSTM results Both approaches demonstrate the ability to capture market trends while highlighting the inherent uncertainty in cryptocurrency markets

## Dataset Overview
### Hyperliquid (HYPE)

- Price Range: $6.42 - $37.44
- Average Volume: 200.83 million
- Market Cap: $6.61 billion (average)
- Data Points: 176 observations
- Volatility: Moderate ($5.56 standard deviation)

### Siacoin (SIA)
- Price Range: $0.001125 - $0.008369
- Average Volume: 26.52 million
- Market Cap: $269.99 million (average)
- Data Points: 364 observations
- Volatility: Low ($0.00115 standard deviation)

### Methodology

- Data Preprocessing: StandardScaler normalization for LSTM input
- Model Architecture: Multi-layer LSTM with dropout regularization
- Pretrained Models: Utilized existing trained models for transfer learning and comparison
- Training Split: 95% training, 5% validation
- Sequence Length: 30-day lookback window
- Evaluation Metrics: MAE (Mean Absolute Error) and RMSE
- Model Ensemble: Combined custom LSTM with pretrained model predictions

## Key Results
### HYPE Forecast

- Prediction: Sideways consolidation at $30-35
- Confidence Interval: $22-50 (80% probability)
- Recommendation: Consider profit-taking at current levels

### SIA Forecast

- Prediction: Gradual recovery to $0.0037-0.004
- Confidence Interval: $0.0025-0.006 (80% probability)
- Recommendation: Attractive entry opportunity at current oversold levels

#### Technologies Used

- Python: Core programming language
- TensorFlow/Keras: LSTM model implementation
- Pandas: Data manipulation and analysis
- Matplotlib: Data visualization
- Scikit-learn: Data preprocessing and scaling
- NumPy: Numerical computations
