# 🏏 Fantasy Cricket Match Winner Prediction  

## 📌 Overview  
This project aims to **predict the winning team in a fantasy cricket match** using **Machine Learning models** trained on **Indian Premier League (IPL) data from 2008 to 2024**. The dataset includes key match statistics such as teams, toss decisions, venues, and winning results.  

## 🔍 Problem Statement  
Fantasy cricket players rely on **historical performance data** to create their teams. This project builds a **predictive model** that helps fantasy cricket users make better team selection decisions based on data-driven insights.  

## 📊 Data Preprocessing & Feature Engineering  
- **Missing Values Handling:**  
  - Filled missing city values for neutral venues (e.g., **Dubai, Sharjah**).  
  - Removed **columns with excessive missing values** (`method`, `target_overs`, `super_over`).  
- **Feature Engineering:**  
  - **Label Encoding:** Converted categorical variables (e.g., `team1`, `team2`, `winner`).  
  - **Outlier Removal:** Used **Interquartile Range (IQR) method** to clean extreme values.  
- **Feature Selection:**  
  - Removed **irrelevant columns** (`match_type`, `target_overs`, `super_over`, `method`).  
  - Selected **important features using Random Forest feature importance ranking**.  

## 🏆 Machine Learning Models & Cross-Validation Performance  
| Model | Cross-Validation Accuracy (%) |  
|--------|----------------------------|  
| Logistic Regression | **21.24%** |  
| Decision Tree Classifier | **46.25%** |  
| Random Forest Classifier | **51.57%** |  
| Support Vector Classifier (SVC) | **13.19%** |  
| **CatBoost Classifier (Best Model) 🏆** | **70.62%** |  
| Gaussian Naïve Bayes | **10.26%** |  
| K-Nearest Neighbors (KNN) | **17.22%** |  

- **Best Model:** ✅ **CatBoost Classifier with 70.62% accuracy** (Before tuning)  
- **Hyperparameter Tuning:** 🎯 **After tuning, accuracy improved to 75%**  

## 📂 Dataset Details  
- **Dataset Name:** IPL Complete Dataset (2008-2024)  
- **Source:** [Kaggle IPL Dataset](https://www.kaggle.com/datasets/saiprudvirajy/indian-premier-league-ipl-2008-2024)  
- **Columns:** Season, Venue, Teams, Toss Decision, Winner, Player of the Match, Result, etc.  

## 📊 Model Evaluation Metrics  
- **Confusion Matrix & Classification Report**  
- **Feature Importance Analysis (Random Forest & CatBoost)**  
- **Cross-Validation Performance Check**  

## 🛠 Technologies Used  
🔹 **Python**  
🔹 **Pandas, NumPy** – Data preprocessing  
🔹 **Matplotlib, Seaborn** – Data visualization  
🔹 **Scikit-Learn, CatBoost, XGBoost** – Machine Learning models  
🔹 **Jupyter Notebook**  

## 🚀 How to Use  
1️⃣ Navigate to the **`Fantasy-Cricket-Predictions`** folder.  
2️⃣ Open the `notebook.ipynb` file in Jupyter Notebook.  
3️⃣ Run the notebook to train models and predict match winners.  

## 📌 Business & Sports Analytics Impact  
📈 This model helps **fantasy cricket players** make informed team selections based on historical IPL data.  
📉 It also provides insights for **sports analysts and betting platforms**.  
