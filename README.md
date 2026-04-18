# Titanic-Survival-Prediction
Titanic Survival Prediction using Machine Learning This project predicts passenger survival using classification algorithms like Logistic Regression, KNN, and Decision Tree. It includes data preprocessing, feature engineering, model comparison, and hyperparameter tuning.
# 🚢 Titanic Survival Prediction (Machine Learning)

## 📌 Project Overview
This project focuses on predicting whether a passenger survived the Titanic disaster using Machine Learning classification techniques.  

It demonstrates the complete ML pipeline from data preprocessing to model evaluation and comparison.

---

## 🎯 Objective
To build and evaluate classification models that can predict passenger survival based on various features such as age, gender, class, and fare.

---

## 📊 Dataset
- Dataset: Titanic Dataset (Kaggle)
- Total Rows: 891
- Features: 12 (before preprocessing)

---

## 🧠 Workflow

### 1. Data Cleaning
- Dropped irrelevant columns: PassengerId, Name, Ticket, Cabin
- Handled missing values:
  - Age → median
  - Embarked → mode

---

### 2. Exploratory Data Analysis (EDA)
- Analyzed survival distribution
- Gender vs Survival → females had higher survival rate
- Passenger class vs Survival → higher class had better survival
- Fare vs Survival → higher fare correlated with survival

---

### 3. Feature Engineering
- Created new feature: `FamilySize`
- Extracted `Title` from Name
- Applied one-hot encoding for categorical variables

---

## 🤖 Models Used

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier
- Hyperparameter Tuned Decision Tree

---

## 📈 Model Performance

| Model                     | Accuracy |
|--------------------------|----------|
| Logistic Regression      | **0.8156** ✅ |
| KNN                      | 0.7207 |
| Decision Tree            | 0.8101 |
| Tuned Decision Tree      | 0.8101 |

---

## 💡 Key Insights

- Gender and passenger class were strong predictors of survival
- Logistic Regression provided the most balanced performance
- Decision Tree initially performed well but required tuning to avoid overfitting
- KNN performed poorly due to sensitivity to feature scaling and data distribution
- Feature engineering (FamilySize, Title) improved model performance

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/titanic-survival-prediction.git

# Navigate to project folder
cd titanic-survival-prediction

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook
