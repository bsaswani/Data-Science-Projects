# 🎭 IMDB Movie Review Sentiment Analysis  

📌 **Overview**  
This project applies **Natural Language Processing (NLP) techniques** to classify IMDB movie reviews as **positive or negative**. The dataset contains **50,000 reviews**, equally balanced between both sentiments. Machine Learning models analyze text features to determine the sentiment of each review.  

🔍 **Problem Statement**  
Movie reviews influence audience decisions and box office performance. This project builds a sentiment analysis model that predicts whether a review expresses **positive or negative** feedback, helping businesses and viewers analyze public opinion.  

📊 **Data Preprocessing & Feature Engineering**  
**Text Cleaning:**  
✔ Converted text to **lowercase**  
✔ Removed **punctuation, special characters, and numbers**  
✔ Eliminated **stopwords** (e.g., "the", "is", "and")  
✔ Applied **stemming** to reduce words to their root forms  

**Feature Engineering:**  
✔ **TF-IDF Vectorization:** Extracted important words & phrases  
✔ **Label Encoding:** Converted sentiment labels to binary values (positive = 1, negative = 0)  

🏆 **Machine Learning Model & Performance**  
| Model | Accuracy (%) |  
|--------------------------|-------------|  
| Logistic Regression | 86% |  

✅ **Best Model:** **Logistic Regression (86%)**  

📂 **Dataset Details**  
- **Dataset Name:** IMDB Movie Reviews  
- **Source:** [Kaggle IMDB Dataset](https://www.kaggle.com/datasets/vishakhdapat/imdb-movie-reviews)  
- **Columns:** Review Text, Sentiment Label  

📊 **Model Evaluation Metrics**  
✔ **Confusion Matrix & Classification Report**  
✔ **Feature Importance Analysis**  
✔ **Cross-Validation Accuracy**  

🛠 **Technologies Used**  
🔹 Python  
🔹 Pandas, NumPy – Data preprocessing  
🔹 Matplotlib, Seaborn – Data visualization  
🔹 Scikit-Learn, NLTK – NLP & ML models  
🔹 Jupyter Notebook  

🚀 **How to Use**  
1️⃣ Navigate to the **IMDB-Sentiment-Analysis** folder.  
2️⃣ Open the `IMDB Movie Review Sentiment Analysis.ipynb` file in **Jupyter Notebook**.  
3️⃣ Run the notebook to train models and classify reviews.  

📌 **Business & Industry Impact**  
📈 Helps movie production companies, review aggregators, and streaming platforms analyze audience sentiment.  
📉 Enables businesses to understand customer feedback and improve services.  
