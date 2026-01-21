# Real Estate Price Analyzer

## Problem Statement
Predict residential property prices using structured housing data
and analyze the key factors influencing sale prices.

## Dataset
Ames Housing Dataset — residential property sales from Ames, Iowa (USA).

## Approach
- Exploratory data analysis with feature-level understanding
- Explicit distinction between structural and true missing values
- Ordinal and nominal feature encoding with semantic preservation
- Baseline linear regression model for reference
- Gradient Boosting Regressor to capture non-linear interactions

## Results
- Linear Regression RMSE (log scale): **~0.174**
- Gradient Boosting RMSE (log scale): **~0.139**  
  (~20% reduction in validation error)

## Key Insights
- Linear models systematically underpredict high-priced properties
- House prices exhibit strong non-linear interactions between
  size, quality, and location
- Gradient Boosting captures these interactions more effectively,
  reducing residual spread for expensive homes

## Limitations
- Single-city dataset (Ames, Iowa)
- No temporal price dynamics
- No external economic or macro-level indicators

## Future Work
- Cross-validation and hyperparameter tuning
- Deeper feature interaction analysis
- Extension to multi-city or regional datasets
