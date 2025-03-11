# 🔥 Fire Detection System (YOLOv8 Nano)  

## 📌 Overview  
This project implements **fire detection** using **YOLOv8 Nano (yolov8n.pt)** for **real-time fire detection in images and videos**. The model is trained on a **custom dataset annotated with CVAT** and is designed for **CCTV surveillance, industrial monitoring, and fire safety systems**.  

## 🔍 Problem Statement  
🔥 Fire detection is critical in **disaster prevention, forest fire monitoring, and building safety**. Traditional methods rely on **sensor-based systems**, but this deep learning approach enables **real-time vision-based fire detection** using cameras.  

## 📊 Data Preprocessing & Feature Engineering  
- **Custom Dataset Annotated Using CVAT** (Computer Vision Annotation Tool).  
- **Resized images to 640x640 pixels** for YOLOv8 model.  
- **Data Augmentation:**  
  - **Brightness Adjustment**  
  - **Blurring**  
  - **Contrast Enhancement**  
- **Converted Bounding Boxes to YOLO Format** for object detection.  

## 🏗️ Deep Learning Model: YOLOv8 Nano  
- **Trained using `yolo8n.pt` (YOLOv8 Nano model)**.  
- **Optimized for real-time detection on edge devices** (low latency).  
- **Detects fire in CCTV, drone footage, and real-world scenarios**.  

### **📊 Model Performance Over Training Epochs**  
| Epoch | Box Loss | Class Loss | DFL Loss | Precision | Recall | mAP50 | mAP50-95 |  
|--------|----------|------------|------------|------------|------------|------------|------------|  
| **28/75** | **1.792** | **2.02** | **1.529** | **0.127** | **0.183** | **0.0605** | **0.0205** |  
| **63/75** | **1.472** | **1.373** | **1.358** | **0.515** | **0.394** | **0.39** | **0.188** |  
| **Final Epoch (75/75)** | **1.365** | **1.298** | **1.243** | **0.678** | **0.569** | **0.541** | **0.322** |  

🔥 **Best Model Performance:**  
- **YOLOv8 Nano achieved 67.8% Precision & 54.1% mAP50** for real-time fire detection.  
- **Optimized for speed and efficiency in embedded systems.**  

## 📂 Dataset Details  
- **Dataset Name:** **Custom Fire Detection Dataset** (Self-Annotated using CVAT).  
- **Image Format:** **640x640 pixels (RGB)**.  
- **Total Images:** **Annotated dataset with fire and non-fire categories**.  

## 📊 Model Evaluation Metrics  
- **Confusion Matrix** – Fire vs. Non-Fire misclassification.  
- **Precision-Recall Curve** – YOLO object detection performance.  
- **Bounding Box Analysis** – Fire detection accuracy in different environments.  

## 🛠 Technologies Used  
- **Python**  
- **YOLOv8 (Ultralytics, PyTorch)** – Object Detection  
- **CVAT (Computer Vision Annotation Tool)** – Dataset Annotation  
- **OpenCV, NumPy** – Image processing tools  
- **Matplotlib, Seaborn** – Data visualization  
- **Jupyter Notebook**  

## 🚀 How to Use  
1️⃣ **Navigate to the `Fire-Detection` folder.**  
2️⃣ **Open `notebook.ipynb` in Jupyter Notebook.**  
3️⃣ **Run the notebook to preprocess images and train the YOLOv8 model.**  
4️⃣ **Use YOLOv8 Nano to detect fire in real-time images and videos.**  

## 📌 Safety & Industrial Impact  
📈 This model can be used in **CCTV surveillance, industrial monitoring, and smart fire detection systems** to enhance **fire safety** in buildings, factories, and forests.  
