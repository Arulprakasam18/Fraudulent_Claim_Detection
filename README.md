# Fraudulent_Claim_Detection

# Fraud Detection in Auto Insurance Claims

This project implements machine learning models to detect fraudulent auto insurance claims using engineered features and balanced datasets. It includes model evaluation, hyperparameter tuning, and insights to support business decision-making.

## Objectives

- Identify fraudulent claims using classification algorithms.
- Interpret model outputs for actionable insights.
- Optimize model performance through feature selection and tuning.

## Techniques and Tools

- **Data Preprocessing:** Encoding, scaling, SMOTE resampling.
- **Feature Selection:** RFECV (Recursive Feature Elimination with Cross-Validation).
- **Models Used:** Logistic Regression, Random Forest, XGBoost.
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score, ROC, AUC.
- **Interpretability:** VIF analysis, model coefficients, feature importance.

## Results Summary

| Model                      | Accuracy | Sensitivity | Specificity | F1-Score |
|---------------------------|----------|-------------|-------------|----------|
| Logistic Regression (0.4) | 0.910    | 0.960       | 0.860       | 0.914    |
| Random Forest (CV Mean)   | 0.923    | -           | -           | -        |

- Important predictors: `total_claim_amount`, `incident_type`, `vehicle_claim`, `policy_incident_duration`.
- Optimal cutoff tuning improved fraud detection (higher sensitivity) while maintaining acceptable specificity.

## Business Impact

- Enables early detection of fraudulent claims to reduce financial losses.
- Enhances customer satisfaction by speeding up legitimate claim processing.
- Supports better allocation of investigation resources.

## Conclusion and Next Steps

- Successfully built and evaluated interpretable and effective fraud detection models.
- Next steps:
  - Deploy the model in production.
  - Monitor model performance.
  - Continuously retrain with updated claim data.
