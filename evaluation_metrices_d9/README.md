# 🧠 Machine Learning Classification Project (Scikit-Learn)

This repository demonstrates a complete **Machine Learning classification workflow** using Python and `scikit-learn`.

It includes:
- Data exploration
- Model training
- Evaluation metrics
- Confusion matrix analysis
- Overfitting detection and improvement

---

# 📌 Dataset Used

### Breast Cancer Wisconsin Dataset (from sklearn)

- **Features:** 30 numeric features (cell measurements)
- **Target:**
  - `0` → Malignant
  - `1` → Benign

---

#  Workflow

1. Load dataset
2. Convert to DataFrame
3. Split data into training and testing sets
4. Train Decision Tree model
5. Make predictions
6. Evaluate model performance
7. Confusion matrix analysis
8. Detect overfitting
9. Improve model using hyperparameters

---

#  Evaluation Metrics

## Accuracy
Measures how many predictions are correct overall.

Accuracy = Correct Predictions / Total Predictions

---

## Precision
Out of predicted positives, how many are correct.

Important when False Positives matter.

---

## Recall
Out of actual positives, how many are correctly detected.

Important when False Negatives are critical (e.g., medical diagnosis).

---

## F1 Score
Harmonic mean of Precision and Recall.

F1 = 2 × (Precision × Recall) / (Precision + Recall)

---

# Confusion Matrix

A confusion matrix compares actual vs predicted results.

| Actual \ Predicted | Positive | Negative |
|--------------------|----------|----------|
| Positive           | TP       | FN       |
| Negative           | FP       | TN       |

Where:
- TP = True Positive
- TN = True Negative
- FP = False Positive
- FN = False Negative

---

# ⚠️ Overfitting

## What is Overfitting?
When a model performs very well on training data but poorly on test data.

### Signs:
- High training accuracy
- Low test accuracy
- Large performance gap

### Cause:
- Model is too complex
- Learns noise instead of patterns

---

## Fixing Overfitting:
- Limit model depth (`max_depth`)
- Use more data
- Cross-validation
- Regularization

---

#  Model Used

Decision Tree Classifier

A **Decision Tree** is a supervised machine learning algorithm used for both **classification** and **regression** tasks.  
It works by splitting data into smaller subsets based on feature conditions, forming a tree-like structure.

---


# 📉Advantages

- Easy to understand and visualize
- No need for feature scaling
- Works with both numerical and categorical data
- Handles non-linear relationships

---

#  Disadvantages

- Prone to overfitting
- Sensitive to small data changes
- Can grow very complex trees


#  Overfitting in Decision Trees

Decision Trees overfit when:
- Tree becomes too deep
- Model memorizes training data
- Learns noise instead of patterns

### Result:
- High training accuracy
- Low test accuracy

---



#  Results Comparison

We compare:
- Training Accuracy
- Test Accuracy

### Interpretation:
- Train ≈ Test → Good model
- Train ≫ Test → Overfitting

---

#  Improvement

To reduce overfitting:
- Controlled tree depth using `max_depth`
- Improved generalization on unseen data

---
