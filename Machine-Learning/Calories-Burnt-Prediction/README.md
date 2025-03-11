# 🔥 Calories Burnt Prediction  

## 📌 Overview  
This project predicts the **calories burned during various physical activities** based on **body metrics (age, weight, height) and exercise intensity (duration, heart rate, MET values).** Using **Machine Learning**, we analyze how different factors contribute to calorie expenditure.  

## 🔍 Problem Statement  
Accurately estimating calorie burn helps in **fitness tracking, personalized workout recommendations, and weight management.** This project builds a predictive model to calculate calories burned based on user attributes and activity levels.  

## 📊 Data Preprocessing & Feature Engineering  
- **Missing Values Handling:**  
  - Checked for missing values and ensured complete dataset integrity.  
- **Feature Engineering:**  
  - **Created new feature `BMI`** from height and weight.  
  - Scaled numerical features using **StandardScaler**.  
- **Outlier Removal:**  
  - Applied **Interquartile Range (IQR) method** to filter extreme values in `Calories_Burnt`, `Heart_Rate`, and `Exercise_Duration`.  

## 🏆 Machine Learning Models & Cross-Validation Performance  
| Model | Cross-Validation R² Score (%) |  
|--------|----------------------------|  
| Linear Regression | **88.79%** |  
| Decision Tree Regressor | **95.12%** |  
| Random Forest Regressor | **98.45%** |  
| Support Vector Regressor (SVR) | **81.73%** |  
| **XGBoost Regressor (Best Model) 🏆** | **99.26%** |  
| K-Nearest Neighbors (KNN) | **90.62%** |  

- **Best Model:** ✅ **XGBoost Regressor with 99.26% accuracy**  
- **Hyperparameter Tuning:** 🎯 **XGBoost improved after tuning**  

## 📂 Dataset Details  
- **Dataset Name:** Calories Burned During Exercise and Activities  
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/aadhavvignesh/calories-burned-during-exercise-and-activities)  
- **Columns:** Age, Weight, Height, Exercise Type, Heart Rate, Duration, MET Value, Calories Burnt  

## 📊 Model Evaluation Metrics  
- **Mean Absolute Error (MAE)**  
- **Mean Squared Error (MSE)**  
- **R² Score** (Regression Performance)  

## 🛠 Technologies Used  
🔹 **Python**  
🔹 **Pandas, NumPy** – Data preprocessing  
🔹 **Matplotlib, Seaborn** – Data visualization  
🔹 **Scikit-Learn, XGBoost** – Machine Learning models  
🔹 **Jupyter Notebook**  

## 🚀 How to Use  
1️⃣ Navigate to the **`Calories-Burnt-Prediction`** folder.  
2️⃣ Open the `notebook.ipynb` file in Jupyter Notebook.  
3️⃣ Run the notebook to train models and predict calories burned.  

## 📌 Fitness & Health Impact  
📈 This model helps **fitness enthusiasts, trainers, and health professionals** accurately track calorie burn based on user-specific data.  
