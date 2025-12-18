# L20: ML Core (EO1)
**Objectives:** Load data, train/test split, linear/logistic regression, evaluate metrics; overfitting/regularization basics.

## Resources
- Scikit-learn tutorials:
  - Linear Regression: https://scikit-learn.org/stable/modules/linear_model.html#ordinary-least-squares
  - Logistic Regression: https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
- Optional: Andrew Ng ML (Coursera audit) Week on linear regression: https://www.coursera.org/learn/machine-learning
- Dataset (direct CSV): Titanic from seaborn repo: https://raw.githubusercontent.com/mwaskom/seaborn-data/master/titanic.csv

## Tasks
- Dataset: use Titanic (Kaggle) or another small CSV.
- Preprocess: select features, handle missing values simply, train/val/test split.
- Train: logistic regression for classification; print accuracy, precision, recall, F1.
- Discuss: overfitting risk; use regularization parameter (C) adjustments.

## Example Code to Analyze
```python
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, stratify=y)
model = LogisticRegression(max_iter=1000)
model.fit(X_train, y_train)
```
What does stratify do? Why set max_iter?

## Knowledge Check
- Difference between accuracy and F1?
- Why split into train/test (and sometimes validation)?
- How does regularization help?

## Exit Criteria
- Script/notebook trains and reports metrics.
- You can explain overfitting and one way to reduce it.
