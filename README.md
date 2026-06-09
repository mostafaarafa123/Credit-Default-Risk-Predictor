#  Credit Default Risk Prediction Pipeline

An end-to-end Machine Learning pipeline designed to predict loan default risks for clients with little or no formal credit history.
This project emphasizes a "Business Problem First" approach, focusing on cost analysis, feature engineering, and robust model evaluation.

##  Project Highlights

* **Business-Centric Metric Selection:** Chose **PR-AUC** over Accuracy as the primary metric to correctly handle a heavy 12:1 class imbalance, acknowledging that False Negatives (missed defaulters) are ~6-10x more expensive than False Positives.
* **Extensive EDA & Anomaly Detection:** Identified and addressed anomalies (e.g., unrealistic `DAYS_EMPLOYED` values) and evaluated feature predictive power using the Kolmogorov-Smirnov (KS) statistic.
* **Advanced Feature Engineering:** Aggregated features across multiple relational tables, generating robust ratio features while maintaining a strict, leakage-free pipeline.
* **Model Optimization & Explainability:** Progressively modeled using Decision Trees, Random Forest, LightGBM, and CatBoost. Performed hyperparameter tuning via **Optuna** and utilized **SHAP** values for deep model explainability.

##  Technical Stack
* **Language:** Python (Jupyter Notebook)
* **Machine Learning:** Scikit-Learn, LightGBM, CatBoost
* **Hyperparameter Tuning:** Optuna
* **Model Explainability:** SHAP
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib

