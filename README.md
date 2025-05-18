# 🚢 Titanic Survival Prediction using Logistic Regression

This project uses **Logistic Regression** to predict whether a passenger survived the Titanic disaster based on features like age, sex, fare, class, and more. It is part of the classic [Kaggle Titanic dataset challenge](https://www.kaggle.com/c/titanic).

---

## 📁 Dataset

- `train.csv`: Used for training the model.
- `test.csv`: Used to generate predictions for submission.

---

## 🧹 Data Cleaning

The following steps were taken:

- Dropped unnecessary columns: `Name`, `Cabin`, `Ticket`, `PassengerId`
- Filled missing values in `Age`, `Fare`, `SibSp`, and `Parch` with the **median**
- Filled missing `Embarked` values with `"U"` (unknown)
- Applied `LabelEncoder` to convert categorical columns: `Sex`, `Embarked`

---

## 🔍 Model

- **Algorithm:** Logistic Regression (`sklearn.linear_model.LogisticRegression`)
- **Data Split:** 80% training / 20% validation
- **Accuracy on Validation Set:** 81.00%

---

## 📦 Requirements

```bash
pip install pandas numpy scikit-learn
``` 
