# Credit Card Fraud Detection Project

This project aims to detect fraudulent credit card transactions using machine learning techniques. Below is a step-by-step explanation of how this was accomplished.

---
Dataset = https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
## 1. Understanding the Dataset

### How Did I Check the Dataset?
- **Look at the Data**: Used `df.head()` to see the first few rows.
- **Dimensions**: Verified the size using `df.shape`.
- **Data Types**: Checked data types and missing values with `df.info()`.
- **Duplicates**: Ensured no duplicate rows with `df.duplicated()`.
- **Target Variable**: Analyzed the `Class` column to check for imbalance.

---

## 2. Preparing the Data

### What Did I Ensure?
1. **No Missing Data**: Verified there were no missing values.
2. **Scaling Features**: Scaled transaction amounts using `StandardScaler`.
3. **Irrelevant Data**: Dropped the `Time` column.
4. **Imbalanced Data**: Checked the imbalance in the `Class` column.

---

## 3. Choosing the Right Model

- **Logistic Regression**: Used as a baseline model.
- **Decision Tree Classifier**: Selected for its ability to handle complex patterns.

---

## 4. Handling Imbalanced Data

- **Undersampling**: Reduced the majority class to balance the dataset.
- **Oversampling (SMOTE)**: Generated synthetic examples of fraud cases to balance the dataset.

---

## 5. Training and Testing

- Split data into training and testing sets.
- Trained and evaluated Logistic Regression and Decision Tree models.
- Metrics used for evaluation:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1 Score**

---

## 6. Saving the Model

- Saved the trained Decision Tree model using `joblib`.
- Demonstrated prediction on a sample transaction.

---

## Key Lessons
1. **Explore Your Data**.
2. **Clean and Prepare**.
3. **Start Simple**.
4. **Evaluate Smartly**.
