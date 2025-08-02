# Titanic-Classification

# Titanic Survival Prediction 🚢

This project predicts whether a passenger survived the Titanic disaster using a Decision Tree Classifier based on demographic and passenger information.

---

## 📝 Problem Statement
The goal is to build a machine learning model that can predict passenger survival based on the following features:
- Pclass (Ticket Class)
- Sex
- Age
- SibSp (No. of Siblings/Spouses aboard)
- Parch (No. of Parents/Children aboard)
- Fare (Ticket Fare)
- Embarked (Port of Embarkation)

---

## 📊 Steps Performed

### 1. Environment Setup
- Created a Jupyter Notebook.
- Installed required Python libraries:
  - pandas
  - numpy
  - scikit-learn

### 2. Data Loading & Exploration
- Loaded `train.csv` into a pandas DataFrame.
- Explored dataset using:
  - `head()`, `info()`, `describe()`
  - Checked for missing values with `isnull().sum()`

### 3. Data Cleaning
- Filled missing **Age** values with the median.
- Filled missing **Embarked** values with the mode.
- Converted categorical columns (**Sex** and **Embarked**) to numeric.

### 4. Feature Selection
Selected the following columns as features for the model:
- Pclass, Sex, Age, SibSp, Parch, Fare, Embarked

Target variable: **Survived**

### 5. Train/Test Split
- Split the dataset into 80% training and 20% testing data.

### 6. Model Training
- Trained a **Decision Tree Classifier** with `max_depth=3` and `random_state=42`.

### 7. Model Evaluation
- Evaluated model performance using:
  - Accuracy Score
  - Classification Report (Precision, Recall, F1-Score)

---
## 🎯 Results
- **Model Accuracy:** **79.89%**

### Classification Report:
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|--------:|
| 0 (Not Survived) | 0.80 | 0.88 | 0.84 | 105 |
| 1 (Survived)     | 0.80 | 0.69 | 0.74 |  74 |

- **Macro Average F1-Score:** 0.79  
- **Weighted Average F1-Score:** 0.80

---
