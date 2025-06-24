# Obesity Predictor (South America)

This project explores the predictive relationship between lifestyle factors (eating habits, physical activity, etc.) and obesity levels in South American populations using machine learning. The dataset includes entries from Mexico, Peru, and Colombia, with synthetic oversampling via SMOTE to ensure balanced class representation.

## Dataset

- Source: Combined real and synthetic data (2,111 entries)
- Target: `NObeyesdad` – Obesity level (multiclass categorical)
- Features used: Lifestyle and demographic data (height/weight excluded)

## Methodology

- Preprocessing: SMOTE used to balance underrepresented obesity classes
- Train-Test Split: 90/10 with fixed random seed for reproducibility
- Models: 
  - Random Forest
  - Support Vector Machine (SVM)
- Evaluation Metrics:
  - Confusion Matrix
  - Top-2 Accuracy (for multiclass evaluation)

## Results

- Random Forest model achieved approximately 88% accuracy on the test set
- Top-2 accuracy provided stronger insight in borderline classification cases

## Limitations

- Does not infer causality — this is a predictive, not explanatory model
- BMI-based labels used as proxies for health status

## Tech Stack

- Python (pandas, scikit-learn, imbalanced-learn)

