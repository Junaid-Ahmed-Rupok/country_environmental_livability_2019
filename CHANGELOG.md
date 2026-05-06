# Changelog

All notable changes to this project will be recorded in this file.

## [1.0.0] - 2025-01-XX

### Added
- Initial release with full 8-section pipeline
- XGBoost classifier with GridSearchCV hyperparameter tuning
- Bootstrap-validated SHAP framework (200 iterations, 95% CI)
- EPI 2020 external validation
- 35+ publication-ready figures (PNG, 300 DPI)
- 4 IEEE-formatted LaTeX tables
- K-Means clustering (K=3) with internal validation metrics
- 5-fold stratified cross-validation across 5 classifiers
- Robustness analysis (outlier removal, partial correlation, group ablation)
- Permutation feature importance tests (2,000 iterations)
- VIF-based multicollinearity filtering
- IterativeImputer for missing value handling
- PCA dimensionality reduction with scree plot and biplot
- Exported labeled dataset: `country_livability_labeled_2019.csv`
- Saved model artifacts: XGBoost `.joblib` + scaler + metadata
- `environment.yml` for reproducible environment setup
- `RESULTS_SUMMARY.txt` quick reference

### Models Evaluated
- Dummy Classifier (baseline)
- Logistic Regression
- Random Forest
- SVC (RBF kernel)
- XGBoost (default + tuned)

### Dataset
- 169 countries, 20 features, year 2019
- 4 feature groups: Environmental, Economic, Social, Governance
- Binary livability labels derived from K-Means clustering
