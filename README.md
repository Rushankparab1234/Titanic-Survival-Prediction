# 🚢 Titanic Survival Prediction using Machine Learning

## 📌 Project Overview

The **Titanic Survival Prediction** project is a supervised machine learning classification project that predicts whether a passenger survived the Titanic disaster based on passenger information such as age, gender, passenger class, fare, and family details.

The project demonstrates a complete machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and feature importance analysis.



## 🎯 Objectives

- Clean missing data (Age and Embarked).
- Encode categorical variables.
- Perform Exploratory Data Analysis (EDA).
- Train multiple classification models.
- Compare model performance using evaluation metrics.
- Identify the most important features affecting survival.
- Save the trained models for future deployment.
- Prepare the project for future Streamlit deployment.





# 📊 Dataset

The dataset contains passenger information from the Titanic disaster.

### Features

| Feature | Description |
|----------|-------------|
| PassengerId | Unique Passenger ID |
| Pclass | Passenger Class (1st, 2nd, 3rd) |
| Name | Passenger Name |
| Sex | Gender |
| Age | Age of Passenger |
| SibSp | Number of Siblings/Spouses |
| Parch | Number of Parents/Children |
| Ticket | Ticket Number |
| Fare | Ticket Fare |
| Cabin | Cabin Number |
| Embarked | Port of Embarkation |
| Survived | Target Variable |

Target Variable

- 0 → Did Not Survive
- 1 → Survived


# 🛠️ Data Preprocessing

The following preprocessing steps were performed:

- Removed the **Cabin** column due to a large number of missing values.
- Filled missing values in **Age** using the median.
- Filled missing values in **Embarked** using the mode.
- Removed unnecessary columns:
  - PassengerId
  - Name
  - Ticket
- Encoded categorical features.
- Applied feature scaling for Logistic Regression.



# 📈 Exploratory Data Analysis

EDA was performed to understand the relationships between different features.

Visualizations include:

- Survival Count
- Survival by Gender
- Survival by Passenger Class
- Age Distribution
- Fare Distribution
- Correlation Heatmap



# 🤖 Machine Learning Models

Three classification algorithms were trained and evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier


# 📊 Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Classification Report
- Confusion Matrix
- ROC Curve



## 📈 Model Performance

| Model | Accuracy | Precision | Recall | ROC-AUC |
|--------|----------|-----------|--------|---------|
| Logistic Regression | **81.01%** | **78.57%** | **74.32%** | **88.24%** |
| Decision Tree | **78.21%** | **72.15%** | **77.03%** | **80.02%** |
| Random Forest | **82.12%** | **80.88%** | **74.32%** | **89.88%** |



# 🏆 Best Performing Model

The **Random Forest Classifier** achieved the best overall performance.

### Performance

- Accuracy : **82.12%**
- Precision : **80.88%**
- Recall : **74.32%**
- ROC-AUC : **89.88%**

Random Forest outperformed the other models by providing the highest accuracy and ROC-AUC score while maintaining a strong balance between precision and recall.



# 📌 Feature Importance

The Random Forest model identified the following features as the most influential:

- Gender (Sex)
- Fare
- Passenger Class (Pclass)
- Age
- Family Size (SibSp, Parch)
- Embarked

These findings align with historical observations of the Titanic disaster, where women, first-class passengers, and passengers who paid higher fares generally had higher survival rates.


# 📷 Project Visualizations

The project includes:

- Survival Count Plot
- Gender vs Survival Plot
- Passenger Class vs Survival Plot
- Age Distribution
- Fare Distribution
- Correlation Heatmap
- Confusion Matrix
- ROC Curve
- Feature Importance Plot



# 💾 Model Saving

The trained models were saved using Joblib.

```python
import joblib

joblib.dump(random_forest_model, "random_forest.pkl")
```


# 🚀 Future Improvements

- Develop a Streamlit web application.
- Hyperparameter tuning using GridSearchCV.
- Cross-validation.
- Model deployment on Streamlit Community Cloud.
- Docker containerization.
- CI/CD pipeline for automated deployment.



# 🧰 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook
- Streamlit (Future Deployment)



# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Titanic_Survival_Prediction.git
```

Navigate into the project

```bash
cd Titanic_Survival_Prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the notebook

```bash
jupyter notebook
```

For future Streamlit application

```bash
streamlit run app.py
```


# 📌 Results

- Successfully cleaned and preprocessed the dataset.
- Built three classification models.
- Compared model performance.
- Identified the most important survival factors.
- Selected Random Forest as the best-performing model.


# 👨‍💻 Author

**Rushank Parab**

AI/ML Enthusiast | Machine Learning | Data Science | Python Developer


## ⭐ If you found this project useful, consider giving it a star!