# AI Stock Prediction System

Streamlit stock prediction app using Yahoo Finance data, a Vanilla LSTM model, and an LSTM + Temporal Attention model.

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Prediction horizon

Choose 1, 3, 5, 10, or 20 trading days in the sidebar. Multi-day forecasts are recursive estimates from the existing models. Future OHLC rows are approximated using predicted close values, and business-day dates do not exclude exchange holidays. Forecasts are for educational/research purposes only and are not financial advice.

## Deploy on Streamlit Community Cloud

Set the main file path to `app.py` and ensure `requirements.txt`, `models/`, `scalers/`, and any needed data/results files are included in the repository. Model files may increase repository size; keep only the required artifacts if platform limits are reached.
