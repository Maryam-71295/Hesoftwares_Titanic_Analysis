🚢 Titanic Survival Prediction – Machine Learning Project
📌 Overview
This project is based on the Titanic - Machine Learning from Disaster challenge. The goal is to build a predictive model to determine whether a passenger survived or not using features like age, gender, class, and fare.

📂 Dataset
Training Set: Used to train the model (includes target variable Survived)
Test Set: Used for predictions (target not provided)

⚙️ Project Workflow
1️⃣ Data Exploration (EDA)
Inspected dataset using .head(), .info(), .describe()
Identified:
Missing values (Age, Cabin, Embarked)
Data types (categorical & numerical)
Analyzed distributions and class imbalance

2️⃣ Data Visualization
Pie charts for:
Survival distribution
Gender, Embarked, Pclass
Histograms for:
Age, Fare, SibSp, Parch
Boxplots:
Detect outliers

Heatmap:
Correlation between numerical features

3️⃣ Data Cleaning
Dropped irrelevant columns:
PassengerId, Ticket, Cabin
Handled missing values:
Age → median (grouped by Pclass & Sex)
Embarked → mode
Fare → median
CabinDeck → filled as “N”

4️⃣ Feature Engineering
Created new features:
FamilySize = SibSp + Parch + 1
Title extracted from Name
CabinDeck from Cabi
Encoded categorical variables:
Label Encoding → Sex, Pclass
One-Hot Encoding → Embarked, CabinDeck

5️⃣ Data Preprocessing
Split dataset into:
Features (X)
Target (y)
Train-test split (80/20)

6️⃣ Model Building
Algorithm used: Random Forest Classifier
Parameters:
n_estimators = 200
max_depth = 6

7️⃣ Model Evaluation
Accuracy: ~83.8%
Metrics used:
Accuracy Score
Classification Report
Confusion Matrix

8️⃣ Visualization of Results
Feature Importance Plot
ROC Curve (AUC Score)
True vs Predicted Comparison

9️⃣ Prediction & Submission
Applied trained model on test dataset
Generated submission file:
final_submission.csv

📊 Key Insights
Female passengers had higher survival rates
First-class passengers had better survival chances
Cabin availability positively influenced survival
Family size and title improved model performance

🚀 Future Improvements
Try advanced models (Gradient Boosting, XGBoost)
Perform hyperparameter tuning
Apply cross-validation
Handle outliers more effectively
Add more feature engineering

🛠️ Tools & Libraries
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn

📎 Conclusion
This project demonstrates the complete machine learning pipeline from EDA to model deployment, achieving strong predictive performance while building core data science skills.
