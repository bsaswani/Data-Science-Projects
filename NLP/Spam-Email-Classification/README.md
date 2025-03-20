# ✉️ Spam Classification of Emails  

📌 **Overview**  
This project builds a **machine learning model** to classify emails as **spam or not spam** using **NLP and classification algorithms**. The dataset consists of **5,728 emails**, labeled accordingly. The goal is to filter unwanted messages and improve email security.  

🔍 **Problem Statement**  
Spam emails account for a large portion of online threats, including **phishing attacks and fraud**. This project develops a **spam detection model** that helps email systems **filter out spam messages efficiently**.  

📊 **Data Preprocessing & Feature Engineering**  
**Text Cleaning:**  
✔ Removed **subject line prefixes** (e.g., "Subject: ")  
✔ Removed **punctuation, numbers, and special characters**  
✔ Applied **stemming** to reduce words to their root forms  

**Feature Engineering:**  
✔ **TF-IDF Vectorization:** Converted emails into numerical data  
✔ **Class Imbalance Handling:** Used **SMOTE** to balance spam vs. non-spam samples  

🏆 **Machine Learning Models & Cross-Validation Performance**  
| Model | Accuracy (%) |  
|--------------------------|-------------|  
| Logistic Regression | 98.6% |    
| Support Vector Machine (SVM) | 98.7% |  

✅ **Best Model:** **SVM (98.7%)**  

📂 **Dataset Details**  
- **Dataset Name:** Spam Email Dataset  
- **Source:** [Kaggle Spam Email Dataset](https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset)  
- **Columns:** Email Text, Spam Label  

📊 **Model Evaluation Metrics**  
✔ **Confusion Matrix & Classification Report**  
✔ **Feature Importance Analysis**  
✔ **Cross-Validation Accuracy**  

🛠 **Technologies Used**  
- **Python**  
- **Pandas, NumPy – Data preprocessing**  
- **Matplotlib, Seaborn – Data visualization**  
- **Scikit-Learn, NLTK – NLP & ML models**  
- **Jupyter Notebook**  

🚀 **How to Use**  
1️⃣ Navigate to the **Spam-Email-Classification** folder.  
2️⃣ Open the `Spam Classification of Emails.ipynb` file in **Jupyter Notebook**.  
3️⃣ Run the notebook to train models and classify emails.  

📌 **Cybersecurity & Industry Impact**  
📈 Helps email providers (Gmail, Outlook, etc.) improve **spam detection algorithms**.  
📉 Reduces the risk of phishing attacks and fraudulent emails for businesses and individuals.  
