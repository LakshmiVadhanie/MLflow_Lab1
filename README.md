# MLflow Lab 1

I've attached the output screenshots reflecting the changes mentioned below in the 'Output screenshots' folder

Changes Made to linear_regression.py

1. Added Random Forest Model for Comparison
- Implemented RandomForestRegressor alongside the original ElasticNet model
- Logs separate parameters: model_type, n_estimators, max_depth
- Creates a second MLflow run for performance comparison
  
Result: Random Forest achieved better R sq score (0.505 vs 0.108)

2. Added Prediction Analysis Function

- Created analyze_predictions() function to provide detailed prediction insights, prints:
  - Prediction range vs actual range
  - Mean error and standard deviation
- Logs 3 additional metrics to MLflow:
  - pred_mean - Mean of predictions
  - pred_std - Standard deviation of predictions
  - residual_std - Standard deviation of residuals (errors)

Result: model evaluation with 6 metrics instead of 3

3. Added Dataset Information Display
- Created print_dataset_info() function
- Displays key dataset statistics:
 - Number of training samples 
 - Number of test samples 
 - Number of features 
 - Target variable range 




