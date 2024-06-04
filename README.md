# Stock-Prediction-DCB
## Subhankar Das
## Overview

The overall workflow to use machine learning to make stocks prediction is as follows:

1. Acquire historical fundamental data – these are the *features* or *predictors*
2. Acquire historical stock price data – this is will make up the dependent variable, or label (what we are trying to predict).
3. Preprocess data
4. Use a machine learning model to learn from the data
5. Backtest the performance of the machine learning model
6. Acquire current fundamental data
7. Generate predictions from current fundamental data

This is a very generalised overview, but in principle this is all you need to build a fundamentals-based ML stock predictor.

run the following in terminal:

```bash
pip install -r requirements.txt
python download_historical_prices.py
python parsing_keystats.py
python backtesting.py
python current_data.py
pytest -v
python stock_prediction.py
```