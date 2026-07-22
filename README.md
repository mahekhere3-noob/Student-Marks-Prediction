# Student Marks Prediction 📚

A **Linear Regression** model that predicts a student's marks based on hours studied, built with `pandas` and `scikit-learn`. Includes a train/test split and model evaluation using Mean Absolute Error (MAE).

This is a beginner-friendly mini project meant to demonstrate the full supervised regression workflow: prepare data → split → train → predict → evaluate.

---

## 📊 Problem Statement

Can we predict a student's marks based on the number of hours they studied?

This project builds a linear regression model on a small dataset of study hours vs. marks scored, then evaluates how well the model generalizes to unseen data using a held-out test split.

---

## 📁 Dataset

| Hours Studied | Marks |
|---|---|
| 2  | 35 |
| 3  | 45 |
| 4  | 50 |
| 5  | 60 |
| 6  | 65 |
| 7  | 72 |
| 8  | 80 |
| 9  | 88 |
| 10 | 95 |

A small, simple dataset that makes the relationship between study hours and marks easy to visualize and interpret.

---

## ⚙️ Approach

1. Load the data into a pandas DataFrame
2. Separate the feature (`Hours`) and the target (`Marks`)
3. Split the data into training and test sets (80/20 split)
4. Fit a `LinearRegression` model on the training set
5. Predict marks for a new value (7.5 hours studied)
6. Evaluate the model on the test set using **Mean Absolute Error (MAE)**

The model learns a line of the form:

```
Marks = m × Hours + c
```

where `m` (slope) and `c` (intercept) are learned automatically from the training data.

---

## 🧠 Tech Stack

- Python 3
- pandas
- scikit-learn

---


## 📈 Result

For a student who studies **7.5 hours**, the model predicts a score of **~76.4 marks**.

On the held-out test set, the model's predictions were off by an average of just **1.21 marks** (MAE) — a strong result on this dataset, though expected given how cleanly linear the data is.

---

## 📝 Note

This project was built as a learning exercise to understand the fundamentals of linear regression, train/test splitting, and model evaluation using scikit-learn.
