# 🎓 Student Performance Analysis  

## 📌 Overview  
This project analyzes **student academic performance** based on various **influential factors** such as **study habits, attendance, parental involvement, and motivation levels.** Using **Machine Learning**, we aim to predict student grades and identify key contributors to academic success.  

## 🔍 Problem Statement  
Understanding the factors that impact student performance is crucial for **educators, policymakers, and parents**. This project builds a predictive model to **classify student grades** and offer actionable insights for improving educational strategies.  

## 📊 Data Preprocessing & Feature Engineering  
- **Missing Values Handling:**  
  - Filled NaN values in `Teacher_Quality`, `Parental_Education_Level`, `Distance_from_Home` using **mode imputation (`fillna()`)**.  
- **Feature Engineering:**  
  - Created **`Grade`** column from **Exam_Score** (A, B, C, D, E).  
  - Encoded categorical variables using **LabelEncoder**.  
- **Outlier Removal:**  
  - Applied **Interquartile Range (IQR) method** to `Hours_Studied`, `Tutoring_Sessions`, `Exam_Score`.  

## 🏆 Machine Learning Models & Cross-Validation Performance  
| Model | Cross-Validation Accuracy (%) |  
|--------|----------------------------|  
| Logistic Regression | **82.27%** |  
| Decision Tree Classifier | **100%** |  
| Random Forest Classifier | **99.95%** |  
| Support Vector Classifier (SVC) | **94.02%** |  
| **CatBoost Classifier (Best Model) 🏆** | **100%** |  
| Gaussian Naïve Bayes | **96.66%** |  
| K-Nearest Neighbors (KNN) | **92.99%** |  

- **Best Model:** ✅ **CatBoost Classifier with 100% accuracy**  
- **Hyperparameter Tuning:** 🎯 **CatBoost achieved 1.0 accuracy after tuning**  

## 📂 Dataset Details  
- **Dataset Name:** Student Performance Factors Dataset  
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors)  
- **Columns:** Hours_Studied, Attendance, Parental_Involvement, Motivation_Level, Exam_Score, etc.  

## 📊 Model Evaluation Metrics  
- **Confusion Matrix & Classification Report**  
- **Feature Importance Analysis (Random Forest & CatBoost)**  
- **Final Accuracy:** **100% on test data**  

## 🛠 Technologies Used  
🔹 **Python**  
🔹 **Pandas, NumPy** – Data preprocessing  
🔹 **Matplotlib, Seaborn** – Data visualization  
🔹 **Scikit-Learn, CatBoost** – Machine Learning models  
🔹 **Jupyter Notebook**  

## 🚀 How to Use  
1️⃣ Navigate to the **`Student-Performance-Analysis`** folder.  
2️⃣ Open the `notebook.ipynb` file in Jupyter Notebook.  
3️⃣ Run the notebook to train models and predict student grades.  

## 📌 Educational Impact  
📈 This model can help **schools, universities, and policymakers** optimize educational strategies.  
📉 It provides insights to **improve student performance based on data-driven recommendations.**  
