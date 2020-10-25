# -Kaggle-Titanic-Predictions
My first Kaggle competition


Data Source is from "train.csv" and "test.csv'

First, run through "Kaggle - Titanic Prediction_Data Analysis.ipynb" using jupyter notebook to have an overview of the relationships between features.

Second, run through "Kaggle - Titanic Prediction_Feature Engineering.ipynb" to do data cleanup on dataset (train and test) which includes missing value imputation, normalising skewed features, categorising ordinal labels etc.
Output data are labelled as "X_train.csv" and "X_test.csv".

All features will be used for predictive analysis of survival for each observation.

Thirdly, run through "Kaggle - Titanic Prediction_Moddel Analysis.ipynb" to generate predictions.
Output data is labelled as Predictions.

Kaggle rated accuracy: 0.77511.

Comments:
For feature engineering, extraction, filling of missing values, grouping categories which represent less than 5% of data in for that variable as rare label and conversion to ordinal categories.
For extraction, the first letter of 'Cabin' was being used for modelling later on.Missing values in continuous numerical variable ('Age') was filled using Impyute - Imputation by Multivariate Imputation by Chained Equations (MICE) while missing values in categorical variables ('Cabin' and 'Embarked') are computed as 'Missing'.For feature selection, all variables were used except 'Name' and 'Ticket'.
For model selection, Decision Trees, Random Forest and Gradient Boosting Decision Trees have been part of the selection process with Random Forest having the highest accuracy score amongst all 3.
