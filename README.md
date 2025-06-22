
# Yes Bank Stock Price Prediction

This project focuses on predicting the closing prices of Yes Bank stock using historical data. We apply multiple regression models and evaluate their performance to find the most accurate approach.

---

## Project Workflow

1. **Data Loading and Cleaning**
2. **Feature Engineering**
3. **EDA & Visualizations**
4. **Model Building**
   - Linear Regression
   - Random Forest (with & without tuning)
   - XGBoost (with & without tuning)
5. **Model Evaluation**
6. **Prediction and Conclusion**

---

##  Dataset Overview

- Source: `dataset.csv`
- Features:
  - `Open`, `High`, `Low`, `Close`, `Date`
- Engineered:
  - `Month`, `Year` (from Date)

> Note: Columns like `Volatility` and `Price_Change` have been removed in this version for simplicity.

---

## Visualization Insights

- Trends of `Close` over time
- Relationships between `Close` and `Open`, `High`, `Low`
- Heatmaps and pairplots to understand feature correlation

---

## Models Evaluated

| Model                   | MAE   | MSE    | R² Score |
|------------------------|-------|--------|----------|
| Linear Regression       | 5.90  | 84.02  | 0.9907  |
| Random Forest           | 8.68  | 196.38 | 0.9783   |
| Random Forest (Tuned)   | 8.68  | 196.38 | 0.9783   |
| XGBoost                 | 9.93  | 223.37 | 0.9753   |
| XGBoost (Tuned)         | 8.80  | 179.07 | 0.9802   |

---

## Conclusion

- **Linear Regression** gave the most accurate prediction in this dataset.
- It had the lowest MAE/MSE and highest R².
- Random Forest and XGBoost were good but not better than Linear Regression here.

---

## Future Scope

- Use technical indicators (MACD, RSI)
- Try deep learning models (LSTM, GRU)
- Deploy using Streamlit or Flask

---

## Tools Used

- Python, Pandas, NumPy
- Scikit-learn, XGBoost
- Matplotlib, Seaborn
