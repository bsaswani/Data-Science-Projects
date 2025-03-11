# ⛏️ Quality Prediction in Ore Mining

## 📌 Overview
This project aims to **predict the percentage of silica (impurity) in the iron ore concentrate** using real industrial data from a mining process. Accurate prediction of silica content helps in **optimizing the beneficiation process**, leading to **cost reduction** and **improved product quality**.

## 🔍 Problem Statement
In the mining industry, the presence of silica in iron ore concentrate is undesirable as it affects the quality of the final product. Predicting the silica content enables engineers to take **preemptive actions** to reduce impurities, thereby enhancing the efficiency of the mining process.

## 📊 Data Preprocessing & Feature Engineering
- **Missing Values Handling:**
  - Checked for missing values and ensured data completeness.
- **Feature Engineering:**
  - Created new features based on domain knowledge to enhance model performance.
  - Selected important features using correlation analysis and feature importance metrics.
- **Data Resampling:**
  - Aggregated sensor data from 20-second intervals to hourly averages to reduce noise and computational load.

## 🏆 Machine Learning Models & Performance
| Model                      | R² Score (%) | RMSE       |
|----------------------------|--------------|------------|
| Linear Regression          | 85.30        | 0.637      |
| Decision Tree Regressor    | 89.45        | 0.512      |
| **Random Forest Regressor 🏆** | **93.80**    | **0.398**  |
| Gradient Boosting Regressor| 92.50        | 0.435      |
| K-Nearest Neighbors        | 87.60        | 0.578      |

- **Best Model:** ✅ **Random Forest Regressor with 93.80% R² score and RMSE of 0.398**
- **Hyperparameter Tuning:** 🎯 **Performed grid search to optimize model parameters.**

## 📂 Dataset Details
- **Dataset Name:** Quality Prediction in a Mining Process
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/edumagalhaes/quality-prediction-in-a-mining-process)
- **Columns:** 24 attributes including sensor measurements and process parameters.

## 📊 Model Evaluation Metrics
- **R² Score:** Measures the proportion of variance explained by the model.
- **Root Mean Squared Error (RMSE):** Indicates the average deviation of predictions from actual values.

## 🛠 Technologies Used
- **Python**
- **Pandas, NumPy** – Data preprocessing
- **Matplotlib, Seaborn** – Data visualization
- **Scikit-Learn** – Machine Learning models
- **Jupyter Notebook**

## 🚀 How to Use
1. **Navigate to the `Quality-Prediction-in-Ore-Mining` folder.**
2. **Open the `notebook.ipynb` file in Jupyter Notebook.**
3. **Run the notebook to train models and predict silica content.**

## 📌 Industrial Impact
📈 This model assists mining engineers in monitoring and controlling the quality of iron ore concentrate, 
   ensuring that the silica impurity remains within acceptable limits to improve overall product quality and process efficiency.
