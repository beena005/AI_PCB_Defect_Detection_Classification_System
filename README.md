# AI_PCB_Defect_Detection_and_Classification_System

## Introduction
This project implements an **AI-based PCB Defect Detection and Classification System** using **image processing** and **deep learning (CNN – ResNet50)**. The system detects, localizes, and classifies PCB defects and provides a **Streamlit-based web application** for real-time visualization of results.

---

## Defects Considered
- Mouse Bite  
- Open Circuit  
- Short Circuit  
- Spur  
- Missing Hole  

---

## 📂 Files Uploaded on GitHub

### 1. Image Processing Code
Implements image preprocessing techniques such as image subtraction, thresholding, contour detection, and ROI extraction to localize PCB defects.

### 2. Training Code
Trains a **ResNet50-based convolutional neural network** for PCB defect classification and evaluates performance using accuracy, loss, and confusion matrix.

### 3. Inference Code
Loads the trained model and performs defect classification on new PCB images, generating predictions with confidence scores.

### 4. Streamlit – App Code
Implements the Streamlit user interface for uploading PCB images and displaying both input and annotated output images.

### 5. Streamlit – Inference Code
Contains the backend inference logic integrated with the Streamlit app to return defect labels, bounding boxes, and confidence scores.

### 6. Streamlit – Requirements File
Lists all Python dependencies required to run the Streamlit application and backend inference pipeline.

### 7. Results Folder
Contains experimental results for each defect type.

---

## 9. How to Run the Streamlit Application

### Step 1: Install Dependencies
```bash
pip install -r requirements.txt
```
### Step 2: Run the Streamlit App
```bash
streamlit run streamlit_app.py
```
### Step 3: Using the Application
1. Upload a PCB image
2. Click Run Detection
3. View:
     - Input image
     - Annotated output image with bounding boxes, defect labels, and confidence scores
     - Table displaying detected defects
4. Download:
     - Annotated output image
     - Detection log file

## Model Performance

### Model Used:ResNet50
### Achieved Accuracy: 99.77% (0.9977)
### Evaluation Metrics:
 - Accuracy and loss plots
 - Confusion matrix
 - Classification report
