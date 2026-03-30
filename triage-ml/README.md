# Triage Predictive Modeling (AITriage4SU)

**Research project**: Machine Learning model for clinical outcome prediction in emergency department triage (UTAD, 2025-2026).

## Technical Implementation

**1. Data Pipeline**
- Processing 500K+ emergency episodes (Manchester Triage System)
- Data quality assessment + validation framework
- Missing data imputation + outlier detection

**2. Feature Engineering**
- Clinical variables engineering (vitals, triage codes, demographics)
- Temporal features from episode timelines
- Interaction terms + polynomial features

**3. Performance Analysis of Manchester Triage System**
- Statistical analysis of triage performance metrics
- Sensitivity/specificity analysis by triage level
- Time-to-treatment compliance rates
- Over/under-triage identification
- Benchmarking against clinical outcomes (admission, mortality)

**4. ML Model Development**
- Supervised classification for outcome prediction
- Model ensemble (XGBoost + Logistic Regression)
- Cross-validation with temporal splits

## Tech Stack
Python | pandas | scikit-learn | XGBoost | SHAP | matplotlib | seaborn


## Outcome
- Identified key predictors for adverse outcomes
- Clinical decision support system prototype
- Data quality improvements recommendations
  
