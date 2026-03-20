# Titanic Survival Prediction

## Overview
This project uses machine learning to predict whether a passenger survived the Titanic disaster. The goal is to understand key factors affecting survival and build a simple predictive model.

---

## Dataset
The dataset contains passenger information such as:
- Age
- Gender
- Ticket Class (Pclass)
- Fare
- Family relationships

Target variable:
- Survived (1 = Survived, 0 = Did not survive)

---

## Approach

### Data Preprocessing
- Selected key features: Pclass, Sex, Age, Fare
- Handled missing values in Age using median
- Converted categorical data (Sex) using one-hot encoding

### Feature Engineering
- Created a new feature **FamilySize**:
  
  FamilySize = SibSp + Parch + 1
  
- This helps capture the effect of traveling with family on survival

---

## Model
- Logistic Regression
- Train-validation split used for evaluation

---

## Results
- Initial accuracy: ~77%
- After fixing missing value handling: **~81% accuracy**

---

## Key Insights
- Female passengers had significantly higher survival rates
- Higher class passengers (Pclass 1) had better survival chances
- Higher fares are associated with higher survival (linked to class)
- Moderate family sizes had better survival compared to very small or very large families
- Age showed weaker influence compared to other factors

---

## Tech Stack
- Python
- Pandas
- Scikit-learn

---

## Conclusion
This project demonstrates how basic preprocessing, feature engineering, and a simple model can produce meaningful insights and reasonable prediction performance.

---

## How to Run
1. Clone the repository
2. Ensure `train.csv` is in the same directory
3. Open the notebook and run all cells
