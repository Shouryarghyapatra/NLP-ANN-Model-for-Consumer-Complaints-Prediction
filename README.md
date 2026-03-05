# 📌 Consumer Complaint Product Classification using Deep Learning

## **📖 Project Overview**

This project develops a deep learning–based Natural Language Processing (NLP) pipeline to classify consumer complaint narratives into their respective product categories. The model learns from textual complaint data and predicts the correct product label using a multi-class classification approach.

The project demonstrates end-to-end implementation of text preprocessing, feature engineering, deep learning model building, and performance evaluation.

---

## **🎯 Problem Statement**

Consumer complaint databases contain thousands of textual narratives describing issues faced by customers. Manually categorizing these complaints is time-consuming and inefficient.

The objective of this project is:

> To automatically classify complaint narratives into predefined product categories using deep learning techniques.

This is a **multi-class text classification problem**.

---

## **📂 Dataset Description**

The dataset contains:

* Complaint narrative text
* Product category labels

Each row represents one consumer complaint.

---

## **⚙️ Project Workflow**

### **1️⃣ Data Cleaning & Preprocessing**

* Removed duplicate entries
* Handled missing values
* Cleaned text using regular expressions
* Converted text to lowercase
* Removed extra whitespace
* Reset dataset indexing

---

### **2️⃣ Label Encoding**

* Converted categorical product labels into numeric format
* Used `LabelEncoder` for multi-class representation

---

### **3️⃣ Text Vectorization**

* Tokenized complaint narratives
* Limited vocabulary size for efficiency
* Converted text into integer sequences
* Applied padding to maintain fixed-length input

---

### **4️⃣ Model Architecture**

The deep learning model consists of:

* **Embedding Layer**
  Learns dense word representations instead of sparse one-hot encoding.

* **Flatten Layer**
  Converts 3D embedding output into a 2D feature vector.

* **Dense Layer (ReLU Activation)**
  Learns hidden patterns in complaint text.

* **Dropout Layer (0.5)**
  Reduces overfitting by randomly disabling neurons during training.

* **Softmax Output Layer**
  Produces probability distribution across multiple product classes.

---

## **🧠 Model Training**

* Train-test split with stratification
* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy
* Evaluation Metrics: Accuracy

---

## **📊 Model Evaluation**

The model performance is evaluated using:

* Accuracy Score
* Confusion Matrix
* Precision
* Recall
* F1-Score

These metrics provide insight into classification performance across different product categories.

---

## **🛠 Tech Stack**

* Python
* Pandas & NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib


