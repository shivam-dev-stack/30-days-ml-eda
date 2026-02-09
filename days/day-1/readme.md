## Dataset Overview

The dataset contains information about Titanic passengers, including:

- Passenger class (Pclass)
- Gender (Sex)
- Age
- Number of siblings/spouses aboard (SibSp)
- Number of parents/children aboard (Parch)
- Fare
- Embarked port
- Survival status (target variable)

Our target variable is **Survived**.


## Missing Value Treatment

The dataset contains missing values, especially in the **Age** column.

- Age is a numerical feature.
- We replace missing values in Age with the **mean age** of passengers.

This is a simple and effective approach for baseline models.


## Feature Selection

For this model, we selected the following features:

- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked

These features are likely to influence survival probability.


## Model Selection: Logistic Regression

Logistic Regression is a simple and interpretable model used for binary classification problems.

Reasons for choosing Logistic Regression:
- Works well as a baseline model
- Easy to interpret
- Fast to train
- Suitable for small to medium datasets


## Model Evaluation Metrics

We evaluate the model using:

- **Accuracy**: Overall correctness of the model
- **Precision**: How many predicted positives are actually correct
- **Recall**: How many actual positives were correctly predicted
- **F1-score**: Balance between precision and recall

These metrics help us understand model performance beyond just accuracy.



## Confusion Matrix Analysis

The confusion matrix results are:

- True Negatives (TN): 91
- False Positives (FP): 14
- False Negatives (FN): 17
- True Positives (TP): 57

### Interpretation

- The model correctly predicts **91 non-survivors**.
- It correctly predicts **57 survivors**.
- It incorrectly predicts **14 passengers as survivors** when they actually died.
- It misses **17 actual survivors**, predicting them as non-survivors.

This shows that:
- The model performs slightly better at predicting non-survivors.
- It has lower recall for the survival class.
- Overall accuracy is around **83%**, which is a good baseline.


## Conclusion

In this project, we built a Logistic Regression model to predict Titanic passenger survival.

### Key results:
- Model accuracy: ~83%
- Balanced performance across both classes
- Logistic Regression provides a strong baseline

### Key insights:
- The model performs slightly better at predicting non-survivors.
- Some survivors are still misclassified, indicating room for improvement.

### Future improvements:
- Try more advanced models like Random Forest or Gradient Boosting
- Perform feature engineering
- Tune hyperparameters