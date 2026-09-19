These contain the trained model artifacts exported by the notebook.

Files

- readmission_model.pkl — Final trained classifier (Logistic Regression).
- scaler.pkl — StandardScaler fitted on the training data.
- feature_info.json — Feature list, selected features, model type, and test metrics.

Notes

The model and scaler must be used together. Load both, scale the input,
then predict. This is for reproducibility and to ensure that the new user will be using the exact model, with the exact same metrics, used in this project.
