# 🧠 Alzheimer MRI Classification  

## 📌 Overview  
This project classifies **Alzheimer’s disease stages** from **MRI brain scans** using a **Convolutional Neural Network (CNN)**. The model detects four categories:  
- **Mild Impairment**  
- **Moderate Impairment**  
- **No Impairment (Healthy Brain)**  
- **Very Mild Impairment**  

## 🔍 Problem Statement  
Early diagnosis of **Alzheimer’s disease** is crucial for treatment and patient care. This deep learning model helps in **automated classification of MRI scans**, reducing human error and improving diagnostic efficiency.  

## 📊 Data Preprocessing & Feature Engineering  
- **Converted images to grayscale** using OpenCV.  
- **Resized images to 100x100 pixels** for uniformity.  
- **Normalized pixel values** to improve model efficiency.  
- **Encoded class labels** using Label Encoding.  
- **Train-Test Split:** **80% training, 20% testing (10,240 images total).**  

## 🏗️ Deep Learning Model (CNN Architecture)  
| Layer Type | Filter/Units | Activation | Output Shape |  
|------------|-------------|------------|--------------|  
| **Conv2D** | 32 filters (3x3) | ReLU | (98, 98, 32) |  
| **MaxPooling2D** | 2x2 | - | (49, 49, 32) |  
| **Conv2D** | 64 filters (3x3) | ReLU | (47, 47, 64) |  
| **MaxPooling2D** | 2x2 | - | (23, 23, 64) |  
| **Flatten** | - | - | (33856,) |  
| **Dense** | 128 neurons | ReLU | (128,) |  
| **Dense (Output Layer)** | 4 neurons | Softmax | (4,) |  

- **Optimizer:** Adam  
- **Loss Function:** Sparse Categorical Crossentropy  
- **Batch Size:** 32  
- **Epochs:** 10  

## 📊 Model Performance  
- **Best Validation Accuracy:** **97.17%**  
- **Evaluation Metrics:**  
  - **Precision:** **97% (Macro Avg)**  
  - **Recall:** **97%**  
  - **F1-score:** **97%**  
  - **Confusion Matrix Analysis:**  
    - **Perfect classification for Moderate Impairment (100%)**  
    - **Minor misclassifications in Very Mild Impairment cases**  

## 📂 Dataset Details  
- **Dataset Name:** Alzheimer MRI Dataset  
- **Image Format:** Grayscale, 100x100 pixels  
- **Total Images:** **10,240** (Train: 8,192 | Test: 2,048)  

## 📊 Model Evaluation Metrics  
- **Confusion Matrix** – Heatmap for misclassifications  
- **Accuracy Score** – Measures overall performance  
- **Classification Report** – Precision, Recall, F1-score  

## 🛠 Technologies Used  
- **Python**  
- **TensorFlow, Keras** – Deep Learning frameworks  
- **OpenCV, NumPy** – Image processing tools  
- **Matplotlib, Seaborn** – Data visualization  
- **Jupyter Notebook**  

## 🚀 How to Use  
1️⃣ **Navigate to the `Alzheimer-MRI-Classification` folder.**  
2️⃣ **Open `notebook.ipynb` in Jupyter Notebook.**  
3️⃣ **Run the notebook to preprocess images and train the CNN model.**  
4️⃣ **Test the model using MRI images for Alzheimer classification.**  

## 📌 Medical Impact  
📈 This model can assist **neurologists, radiologists, and researchers** in the early detection of **Alzheimer’s disease**, leading to **better patient management and treatment planning.**  
