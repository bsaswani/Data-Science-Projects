# 🏥 Medical Insurance Cost Prediction

## 📌 Overview
This project aims to **predict individual medical insurance costs** using **Machine Learning models** trained on personal health data. The dataset includes features such as age, sex, BMI, number of children, smoking status, and region.

## 🔍 Problem Statement
Accurately predicting medical insurance costs is crucial for **insurance companies** to set fair premiums and for **individuals** to understand potential expenses. This project builds a predictive model to estimate insurance charges based on personal attributes.

## 📊 Data Preprocessing & Feature Engineering
- **Missing Values Handling:**
  - Verified that the dataset has no missing values.
- **Feature Engineering:**
  - **One-Hot Encoding:** Converted categorical variables (`sex`, `smoker`, `region`) into numerical format.
- **Outlier Detection:**
  - Analyzed distributions to identify and handle potential outliers in `bmi`, `age`, and `charges`.

## 🏆 Machine Learning Models & Performance
| Model                      | R² Score (%) | RMSE       |
|----------------------------|--------------|------------|
| Linear Regression          | 75.42        | $4,576.70  |
| Decision Tree Regressor    | 71.36        | $4,942.29  |
| Random Forest Regressor    | 84.52        | $3,501.41  |
| Support Vector Regressor   | 76.89        | $4,431.23  |
| **XGBoost Regressor 🏆**   | **85.67**    | $3,376.45  |
| K-Nearest Neighbors        | 72.15        | $4,860.12  |

- **Best Model:** ✅ **XGBoost Regressor with 85.67% R² score and RMSE of $3,376.45**
- **Hyperparameter Tuning:** 🎯 **Performed grid search to optimize model parameters.**

## 📂 Dataset Details
- **Dataset Name:** Medical Cost Personal Datasets
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Columns:** `age`, `sex`, `bmi`, `children`, `smoker`, `region`, `charges`

## 📊 Model Evaluation Metrics
- **R² Score:** Measures the proportion of variance explained by the model.
- **Root Mean Squared Error (RMSE):** Indicates the average deviation of predictions from actual values.

## 🛠 Technologies Used
- **Python**
- **Pandas, NumPy** – Data preprocessing
- **Matplotlib, Seaborn** – Data visualization
- **Scikit-Learn, XGBoost** – Machine Learning models
- **Jupyter Notebook**

## 🚀 How to Use
1. **Navigate to the `Medical-Insurance-Cost-Prediction` folder.**
2. **Open the `notebook.ipynb` file in Jupyter Notebook.**
3. **Run the notebook to train models and predict insurance costs.**

## 📌 Business Impact
📈 This model assists **insurance companies** in setting accurate premiums and helps **individuals** anticipate medical expenses based on personal health factors.
