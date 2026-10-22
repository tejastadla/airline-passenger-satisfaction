# Airline Passenger Satisfaction Classifier

Predicts whether an airline passenger is satisfied, using 130K survey records.

**Dataset:** Airline Passenger Satisfaction (Kaggle). To run the notebook, download `train.csv` and `test.csv` into a `data/` folder next to it.

## What it does
- Cleans the data, encodes categorical columns, and engineers Total Delay and Avg Service Rating
- Explores the data with plots of satisfaction by class, delays, and service-rating correlations
- Compares Logistic Regression, Decision Tree, and Random Forest, tuned with GridSearchCV
- Groups passengers into service-experience segments with PCA and K-Means clustering
- Ranks the top drivers of satisfaction using Random Forest feature importance

## Results (test set)
| Model | Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | 0.8710 | 0.9253 |
| Decision Tree | 0.9542 | 0.9739 |
| Random Forest | 0.9618 | 0.9936 |

## Tech
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn


