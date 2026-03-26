# Movie Revenue Analysis & Regression

This project aims to analyze movie dataset features and build regression models to predict movie revenue. It includes data preprocessing, exploratory data analysis (EDA), and initial insights on feature-target relationships.

## Dataset
The dataset contains information about movies including budget, popularity, runtime, revenue, cast & director scores, language, release details, and collections.

**Key Columns:**
- Numerical: `budget`, `popularity`, `runtime`, `revenue`, `cast_score`, `director_score`, etc.
- Categorical/Binary: `has_collection`, `has_homepage`, `original_language`, `release_month`, `release_dayofweek`, `genre_count`

## Data Preprocessing
- Handled missing values in numerical and categorical columns.
- Encoded categorical features (`has_collection`, `original_language`, etc.) using one-hot encoding.
- Created new features like `director_score`, `cast_score`, `keyword_score`.
- Log-transformed skewed numerical columns (`budget`, `revenue`) for better model performance.
- Feature scaling where necessary.

## Exploratory Data Analysis
- **Univariate Analysis:** Histograms and boxplots of `revenue`, `budget`, `popularity`, etc.
- **Bivariate Analysis:** Revenue vs categorical features (`has_collection`, `original_language`) and numerical features (`budget`, `popularity`).
- **Correlations:** Strong positive correlation observed between `budget` and `revenue`.
- Identified outliers and skewness in numerical features.

## Next Steps
- Implement regression models to predict movie revenue:
  - Start with Linear Regression (parametric baseline)
  - Then explore Random Forest and Gradient Boosting (non-parametric models)
- Evaluate models using R², RMSE, and MAE.
- Perform feature importance analysis to identify key factors influencing revenue.

## Tools & Libraries
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
- Jupyter Notebook for EDA and preprocessing
