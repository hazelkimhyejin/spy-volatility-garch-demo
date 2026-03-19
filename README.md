# SPY Volatility Forecasting with GARCH(1,1)

Small demonstration project for quant researcher applications.

- Daily SPY data (2015–2026) via yfinance
- EDA + ARCH effects test
- GARCH(1,1) fit (zero mean)
- Rolling 1-day-ahead volatility forecasts
- Comparison vs naive historical MA benchmark
- Evaluation: MAE / RMSE using |returns| as realized vol proxy

**Key takeaway**: GARCH captures volatility clustering and persistence (α + β ≈ 0.98).  
On this run, naive benchmark slightly better in MAE — typical for noisy daily proxies; GARCH often superior under proper scoring or longer horizons.

**Next steps**: EGARCH/GJR for leverage effect, QLIKE loss, LSTM/XGBoost comparison, high-freq realized vol.

Built in Jupyter/Colab with `arch`, `yfinance`, `pandas`.
