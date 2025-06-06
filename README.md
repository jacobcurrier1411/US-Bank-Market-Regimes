# Market Regime & Fragility Analysis of U.S. Bank Stocks (2006–2025)

This project explores regime shifts and systemic fragility in the U.S. banking sector using unsupervised learning and financial risk modeling techniques. By combining technical indicators, macroeconomic features, and fundamental data, the notebook identifies patterns of stress across major U.S. banks and produces early warning signals for crisis periods.

---

## Project Highlights

- KMeans clustering of bank stock features to detect 3 market regimes:
  - Growth
  - Slowdown
  - Crisis
- Engineered features:
  - Rolling returns, volatility, skewness, and drawdown for 6 major banks
  - Fed Funds Rate, CPI, and Unemployment from FRED
- Fragility Score:
  - Calculated via Mahalanobis distance from baseline "normal" conditions
  - Quantifies systemic stress across time
- Early Warning Signals:
  - Flags periods of elevated fragility before known crises (2008, 2020)
  - Visualizes stress buildup and recovery phases
- Correlation Analysis:
  - Rolling pairwise return correlations reveal contagion patterns during crises

---

## Tools and Libraries

- Python 3, Jupyter Notebook  
- pandas, numpy – data preparation and time series analysis  
- scikit-learn – KMeans clustering, StandardScaler  
- matplotlib, seaborn – visualization  
- scipy – Mahalanobis distance and statistical measures  
- Data from: Yahoo Finance and FRED (Federal Reserve Economic Data)

---

## Files

| File | Description |
|------|-------------|
| `MarketRegimeUSBanks.ipynb` | Full project notebook with code, charts, and markdown commentary |
| `MarketRegimeUSBanks.pdf` | Exported PDF version for non-technical reviewers |
| `fragility_chart.png` | Sample fragility score output showing early warning periods |

---

## Insights and Takeaways

- Crisis regimes are clearly distinguishable using unsupervised learning on engineered features.
- Fragility scoring surfaces abnormal stress weeks aligned with historical crisis events.
- Early warning thresholds successfully identified fragility ahead of 2008 and 2020 events.
- This framework can be adapted for other sectors or regions for systemic risk monitoring.

---

## Author

**Jacob Currier**  
Finance Graduate | Python & Data-Driven Investment Analysis  
[LinkedIn](https://www.linkedin.com/in/jacob-currier10/)  
jacob.currier@marist.edu

---

## License

This project is for educational and portfolio demonstration purposes only. Data is sourced from public APIs under fair-use terms.
