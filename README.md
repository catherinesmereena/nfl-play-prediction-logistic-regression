# nfl-play-prediction-logistic-regression
Logistic and stepwise regression models to classify NFL plays as Run or Pass using game state features like down, distance, and field position.

 NFL Play Type Prediction Using Logistic Regression

This project applies Logistic and Stepwise Logistic Regression models to predict whether an NFL play will be a pass or a run. Developed for the ALY6020 Predictive Analytics course at Northeastern University, this model offers insights into play-calling strategies based on game conditions.

##  Objective
To classify NFL play types using structured game data and evaluate how game dynamics (e.g., down, yard line, time remaining) influence play-calling decisions.

##  Data Preparation
- Removed irrelevant columns and handled missing values using mode imputation
- Standardized numeric features and encoded categorical ones
- Engineered features like `IS_RED_ZONE`, `ABS_SCORE_DIFFERENTIAL`, and `REMAINING_TIME_SECONDS`
- Applied VIF analysis to eliminate multicollinearity

##  Modeling & Evaluation
- Built baseline Logistic Regression and refined with Stepwise Logistic Regression
- Accuracy: **60.1%**
- Higher precision in predicting passing plays; higher recall for running plays
- Top predictors: `TO GO`, `DOWN`, `YARD LINE 0-100`

##  Files Included
- `ALY6020_Assignmnet3_week3_.ipynb`: Code for preprocessing, modeling, and evaluation
- `ALY6020_FootBall Data Analysis_week3.docx`: Written report
- `Training_Data-1.xlsx`: Training dataset
- `test_results (1).csv`: Test set predictions

##  Tools & Libraries
- Python, Pandas, Scikit-learn, Statsmodels
- Matplotlib, Seaborn
- Jupyter Notebook

##  Key Takeaways
- Logistic regression provides interpretable predictions for play calling
- Stepwise selection helps refine features for better generalizability
- Further improvements can include non-linear models or additional player-level features
