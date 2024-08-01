<h1 align="center">Project: Credit Card Fraud Detection Analysis</h1>


**Description:** The objective of this project is to learn how to deal with an unbalanced dataset of credit card fraud transactions and build a classifier model that can identify the fraudulent. One of the greatest challenges while working on this project is deciding how to calculate the model's accuracy.

**Data Source:** [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

**Libraries:**
- Pandas
- Seaborn
- Sklearn model selections (*GridSearchCV & cross_val_score*)
- Sklearn ML libraries (*linear_model, svm, neighbors & tree*)

**Sections Covered:**
- Data Pre-processing/Data Cleaning
- Data Exploration
- Undersampling Skewed Dataset
- ML Model Selection
- Accuracy Score using ROC (ROC curves should be used when there are roughly equal numbers of observations for each class)

**Data Visualizations Preview:**

![viz preview](https://github.com/alyani-fr/DataSciencePortfolio/assets/88192027/063006bf-3baa-4c20-862e-c8ed4d39dc1d)

**Conclusions:**
- The dataset has 99.83% of legit transactions and 0.17% of fraud transactions.
- Use undersampling of the majority data where the new sample data consists of a normal distribution between the legit and fraud transactions.
- Using cross validation to check for models accuracy and found that, LogisticRegression has  94.0 % accuracy score, SVC has  53.0 % accuracy score, DecisionTreeClassifier has  90.0 % accuracy score and, KNeighborsClassifier has  62.0 % accuracy score.
- Best parameters selection for logistic regression with GridSearchCV where the best parameters obtained in the grid search: Penalty = l2 and C = 0.166.
- Using the best params from GridSearchCV to build the logistic regression, resulting in Area under ROC: 0.96, Accuracy: 0.93, Precision: 0.95 and Recall: 0.91.
