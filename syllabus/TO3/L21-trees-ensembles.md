# L21: Trees and Ensembles (EO1)
**Objectives:** Train decision trees and random forests/GBMs; compare metrics and overfitting control.

## Resources
- Scikit-learn decision trees: https://scikit-learn.org/stable/modules/tree.html#classification
- RandomForestClassifier: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
- Video: Decision trees and overfitting (StatQuest ~12m): https://www.youtube.com/watch?v=_L39rN6gz7Y

## Tasks
- Train a decision tree and random forest on the same dataset as L20.
- Compare metrics to logistic regression.
- Adjust hyperparameters: depth, min_samples_leaf; observe over/underfitting.
- View feature importances and interpret top features.

## Example Code to Analyze
```python
from sklearn.ensemble import RandomForestClassifier
rf = RandomForestClassifier(n_estimators=200, max_depth=None, random_state=0)
rf.fit(X_train, y_train)
```
Why does a forest reduce variance compared to a single tree?

## Knowledge Check
- What causes trees to overfit?
- How do ensembles help generalization?
- When prefer tree-based models over linear?

## Exit Criteria
- Notebook/script showing metrics for tree vs forest vs logistic.
- Short note on best-performing model and why.
