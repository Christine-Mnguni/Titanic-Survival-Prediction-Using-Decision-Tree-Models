# 🛳️ Titanic Survival Prediction Using Decision Tree Models

# 📌 Project Overview
This project builds and evaluates tree-based classification models to predict the survival of passengers aboard the Titanic using historical passenger data. We explore three ensemble learning methods — Bagging, Random Forest, and Gradient Boosting — to compare their predictive performance and identify the most accurate model.

# 📁 Dataset
The dataset is based on the Titanic passenger list and includes features like:

Pclass: Ticket class (1st, 2nd, 3rd)

Sex: Gender of the passenger

Age: Age in years

SibSp: Number of siblings/spouses aboard

Parch: Number of parents/children aboard

Fare: Ticket fare

Embarked: Port of embarkation (C, Q, S)

Survived: Survival outcome (target variable)

# 🛠️ Methodology
# 1. Data Preparation
Handled missing values in Age and Embarked.

Encoded categorical features (Sex, Embarked).

Selected meaningful features for prediction.

Split the data into training, development, and test sets (60/20/20 split).

# 2. Model Training and Evaluation
# ✅ Models Trained:
Bagged Trees using BaggingClassifier

Random Forest using RandomForestClassifier

Boosted Trees using GradientBoostingClassifier

# 📊 Metrics:
Accuracy on the development set was used for model comparison.

The best model was further evaluated on the test set.

# 3. Hyperparameter Tuning
Tested combinations of n_estimators and max_depth for the Random Forest model.

Selected parameters that gave the highest development accuracy.

# 4. Feature Importance
Identified key predictors of survival using the Random Forest’s feature importance scores.

#  ✅ Results Summary
Model	Development Accuracy
Bagged Trees	~XX.XX%
Random Forest	~XX.XX%
Boosted Trees	~XX.XX%
Best RF Model	n_estimators={n}, max_depth={depth}
Test Accuracy	~XX.XX%

Replace the XX.XX%, {n}, and {depth} with your actual results.

# 📈 Key Insights
Random Forest consistently performed the best across both development and test sets.

Sex, Fare, and Pclass were among the most important predictors of survival.

Ensemble tree-based methods significantly outperform individual decision trees.

# 🔧 Libraries Used
pandas, numpy – Data manipulation

matplotlib, seaborn – Visualization

sklearn – Machine learning models and evaluation

# 💡 Future Improvements
Perform cross-validation for more robust evaluation.

Tune additional hyperparameters (e.g., min_samples_split, min_samples_leaf).

Compare with logistic regression and non-tree-based models.

Address class imbalance using SMOTE or class weights.

