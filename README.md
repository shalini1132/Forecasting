# LSTM Time Series Forecasting – Energy Dataset

This repository presents a deep learning approach for multivariate time series forecasting using Long Short-Term Memory (LSTM) networks. The project evaluates forecasting accuracy and explains model predictions using SHAP (SHapley Additive exPlanations).

---

## 🚀 Project Structure

- `LSTM_SHAP_Forecasting.ipynb` — Main Colab notebook for modeling, training, evaluation, and SHAP analysis.
- `model_evaluation_report.md` — Detailed metrics, plots, and baseline comparisons.
- `Feature_Importance_Summary.md` — SHAP summary and interpretation of feature impact.
- `actual_vs_predicted.png` — Prediction plot image.
- `shap_summary_plot.png` — SHAP global feature importance plot image.
- `shap_force_plot.png` — SHAP force plot (local explanation for a single sample).
- `time_series_dataset.csv` — Source data.

---

## 📈 Methodology

1. **Data Preparation:**  
   - Multivariate time series dataset with lag features and weather variables.
   - Train-test split and normalization.

2. **Modeling:**  
   - LSTM network trained to predict future energy usage.
   - Benchmarked against Naive, ARIMA, and Exponential Smoothing.

3. **Evaluation:**  
   - RMSE, MAE, and MAPE reported for all models.
   - Prediction accuracy visualized.

4. **Explainability (SHAP):**  
   - SHAP summary plot ranks the most important features.
   - SHAP force plot visualizes how features contributed to one prediction.

---

## 📊 Results

- **LSTM significantly outperforms classic baselines** for RMSE and MAE.
- **Key drivers:** Lag features (especially Lag_1), temperature, humidity.
- **Model transparency improved** by SHAP visualizations.

![Actual vs Predicted](actual_vs_predicted.png)
![SHAP Feature Importance](shap_summary_plot.png)
![SHAP Force Plot](shap_force_plot.png)

---

## 📝 Usage

1. Open and run `LSTM_SHAP_Forecasting.ipynb` in Google Colab.
2. Update/configure data path if needed.
3. All key results and exported images appear in the notebook and can be found in the files sidebar.
4. Reports in `.md` files document model metrics, plots, and interpretations.

---

## 📚 References
- [SHAP Documentation](https://github.com/slundberg/shap)
- [Keras LSTM Documentation](https://keras.io/api/layers/recurrent_layers/lstm/)
- [Energy/Time Series Dataset Source](#)

---
