# Fraud Detection – Imbalanced Classification (R + Python)

Two-part imbalanced classification project built as part of a Statistical Analysis course.
Part 1 builds a statistical model + Monte Carlo evaluation.
Part 2 evaluates sampling techniques + ML algorithms for minority fraud detection.

## Goal

* Study how severe class imbalance affects model performance
* Quantify the failure of naïve accuracy on imbalanced data
* Evaluate whether rebalancing strategies improve minority fraud detection

## Methods

* **Languages:** R (Part 1) + Python (Part 2)
* **Part 1:** Monte Carlo simulation evaluating logistic regression under severe class imbalance
* **Part 2:** compare sampling approaches:
  * SMOTE
  * Random Oversampling
  * Random Undersampling
* **Algorithms evaluated:** Logistic Regression, SVM (linear kernel), Random Forest, Gradient Boosting
* Metrics compared emphasize minority class performance (sensitivity / recall)

## Repo Structure

```
.
├─ notebooks/
│   ├─ fraud-part1.Rmd       # statistical model + Monte Carlo study (R)
│   └─ fraud-part2.ipynb     # sampling + ML model comparison (Python)
└─ data/                     # dataset
```

## Deliverables

* `notebooks/fraud-part1.Rmd` — statistical model + Monte Carlo evaluation (R)
* `notebooks/fraud-part2.ipynb` — sampling strategies + ML performance comparison (Python)

## Result Summary

Part 1 shows very high accuracy does **not** imply minority class detection. Logistic regression almost perfectly predicts the majority class but performs poorly on fraud.

Part 2 shows that oversampling strategies, especially SMOTE and random Oversampling, substantially improve minority class sensitivity, with **Random Forest** and **Gradient Boosting** consistently performing best across rebalancing methods.
