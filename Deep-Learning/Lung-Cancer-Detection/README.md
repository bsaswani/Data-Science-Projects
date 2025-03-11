# 🫁 Lung Cancer Detection  

## 📌 Overview  
This project classifies **lung cancer types** using **CT scan images** and a **CNN-based deep learning model**. The model detects four categories:  
- **Adenocarcinoma**  
- **Large Cell Carcinoma**  
- **Normal (Non-Cancerous Scans)**  
- **Squamous Cell Carcinoma**  

## 🔍 Problem Statement  
Lung cancer is one of the **leading causes of cancer-related deaths worldwide**. Early and accurate classification of lung cancer types helps in **better treatment planning and patient survival rates**. This model automates **cancer classification** using **CT scan image analysis**.  

## 📊 Data Preprocessing & Feature Engineering  
- **Converted images to NumPy arrays and normalized pixel values (`0-1`).**  
- **Resized images to 110x110 pixels** for uniformity.  
- **Encoded class labels** into numerical values using Label Encoding.  
- **Train-Test Split:** **80% training, 20% testing**.  

## 🏗️ Deep Learning Model (CNN Architecture)  
| Layer Type | Filter/Units | Activation | Output Shape |  
|------------|-------------|------------|--------------|  
| **Conv2D** | 32 filters (3x3) | ReLU | (108, 108, 32) |  
| **MaxPooling2D** | 2x2 | - | (54, 54, 32) |  
| **Conv2D** | 64 filters (3x3) | ReLU | (52, 52, 64) |  
| **MaxPooling2D** | 2x2 | - | (26, 26, 64) |  
| **Conv2D** | 128 filters (3x3) | ReLU | (24, 24, 128) |  
| **MaxPooling2D** | 2x2 | - | (12, 12, 128) |  
| **Flatten** | - | - | (18432,) |  
| **Dense** | 128 neurons | ReLU | (128,) |  
| **Dense (Output Layer)** | 4 neurons | Softmax | (4,) |  

- **Optimizer:** Adam  
- **Loss Function:** Sparse Categorical Crossentropy  
- **Batch Size:** 32  
- **Epochs:** 13  

## 📊 Model Performance  
| **Epoch** | **Accuracy** | **Validation Accuracy** | **Loss** | **Validation Loss** |  
|------------|--------------|----------------------|----------|------------------|  
| **1/13**  | **28.1%** | **39.8%** | **1.3891** | **1.2226** |  
| **5/13**  | **86.4%** | **83.7%** | **0.3663** | **0.5105** |  
| **10/13** | **98.8%** | **87.8%** | **0.0478** | **0.4980** |  
| **Final (13/13)** | **99.5%** | **86.9%** | **0.0584** | **0.7992** |  

📈 **Best Performance:** **99.5% accuracy on training set, 86.9% validation accuracy.**  

## 📂 Dataset Details  
- **Dataset Name:** **Lung Cancer CT Scan Dataset**  
- **Image Format:** **110x110 pixels (RGB)**  
- **Total Images:** **613 (Train: 490 | Test: 123)**  

## 📊 Model Evaluation Metrics  
- **Confusion Matrix** – Measures correct vs. incorrect predictions.  
- **Precision-Recall Curve** – Highlights classification accuracy.  
- **Classification Report** – Precision, Recall, F1-score.  

## 🛠 Technologies Used  
- **Python**  
- **TensorFlow, Keras** – Deep Learning frameworks  
- **OpenCV, NumPy** – Image processing tools  
- **Matplotlib, Seaborn** – Data visualization  
- **Jupyter Notebook**  

## 🚀 How to Use  
1️⃣ **Navigate to the `Lung-Cancer-Detection` folder.**  
2️⃣ **Open `notebook.ipynb` in Jupyter Notebook.**  
3️⃣ **Run the notebook to preprocess images and train the CNN model.**  
4️⃣ **Test the model using CT scan images for lung cancer classification.**  

## 📌 Medical Impact  
📈 This model can assist **radiologists and oncologists** in the early detection of **lung cancer**, leading to **better treatment and improved patient outcomes**.  
