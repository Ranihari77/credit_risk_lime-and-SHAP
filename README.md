# credit_risk_lime-and-SHAP

Interpretable Credit Risk Assessment using XGBoost, SHAP, and LIME
This project builds an interpretable machine-learning model for credit-risk prediction using a synthetic dataset.  
The model predicts loan default and provides explainability using SHAP (global + local) and LIME (local rule-based explanations).
 Files Included
- credit_risk_lime_and_shap.ipynb — full code (data generation, preprocessing, model training, SHAP & LIME)
- shap_summary.png — global SHAP summary plot
- shap_bar.png — global SHAP bar chart
- shap_force_approval.png — SHAP force plot (approval case)
- shap_force_denial.png — SHAP force plot (denial case)
- shap_force_borderline.png — SHAP force plot (borderline case)
- lime_approval.csv — LIME explanation (approval)
- lime_denial.csv — LIME explanation (denial)
- lime_borderline.csv — LIME explanation (borderline)
- lime_combined.csv — combined LIME outputs
- README.md — project documentation

 Model Summary
- Model used: XGBoost
- Evaluation Metrics (Test Set):  
  - Accuracy ≈ 0.968  
  - Precision ≈ 0.965  
  - Recall ≈ 0.944  
  - F1-score ≈ 0.954  
  - AUC ≈ 0.996  

 Explainability Summary
- Global SHAP identifies top drivers of default risk (e.g., risk_burden, credit_utilization, previous_defaults).
- Local SHAP & LIME provide explanations for three cases: approval, denial, borderline.
 How to Run
1. Open the notebook credit_risk_lime_and_shap.ipynb (Colab recommended).
2. Run all cells — all plots and LIME CSV files will be generated automatically.
