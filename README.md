
## 🌤️ Project Overview

This project is a **Weather Prediction Website** similar to **nsm.com**, built using a custom machine learning pipeline and a curated dataset. The system predicts weather conditions for different cities using algorithms such as **CART**, **Naive Bayes**, and **Clustering**, enabling users to analyze and interpret local weather behavior.

The platform provides:

* City‑wise weather predictions
* Detailed ML‑based insights
* A structured backend pipeline for data preprocessing, model training, and prediction
* A simple frontend for user interaction

This repository contains the complete source code including dataset preprocessing, model files, scripts, and frontend UI.

---

## 🧠 Machine Learning Models Used

### 1. **CART (Classification and Regression Trees)**

* Used for predicting **categorical** (Sunny/Rainy) or **numerical** values (Temperature)
* Performs recursive partitioning on features
* Helps identify the most impactful factors affecting weather

### 2. **Naive Bayes Classifier**

* Suitable for probabilistic predictions
* Classifies weather conditions based on prior and likelihood
* Works well even with limited or noisy data

### 3. **Clustering (K‑Means / Hierarchical)**

* Groups weather patterns based on similarity
* Helps identify seasonal behavior
* Useful for unsupervised weather trend analysis

---

## 🛠️ Technologies Used

### **Backend / ML**

* Python 3.x
* NumPy
* Pandas
* Scikit‑learn
* Matplotlib (for graphs)

### **Frontend**

* HTML5
* CSS3
* JavaScript

### **Tools / Environment**

* Jupyter Notebook / VS Code
* GitHub for versioning
* CSV dataset for model training

---

## ⚙️ Project Functionalities

### ### 🔹 **1. Data Preprocessing**

* Reads raw CSV dataset
* Cleans missing values
* Normalizes numerical features
* Converts text labels to numerical format

### 🔹 **2. Model Training**

Each ML model is trained using preprocessed data.

* CART → generates a decision tree
* Naive Bayes → generates class probability tables
* Clustering → creates weather clusters

Trained models are saved for reuse.

### 🔹 **3. Prediction Engine**

The website takes the following inputs:

* City
* Temperature
* Humidity
* Pressure
* Wind speed

Then the backend returns:

* Predicted weather condition (Sunny/Rainy/Cloudy)
* Probability scores (for Naive Bayes)
* Cluster group mapping

### 🔹 **4. Web Interface**

The frontend includes:

* A simple form to enter city and parameters
* A results section showing predictions
* Clear visualization of temperature trends

### 🔹 **5. Visualization Dashboard**

* Plots temperature/humidity graphs
* Shows cluster visualization
* Displays classification boundaries (optional)

---

## 📁 Repository Structure

```
project-root/
│── data/
│   └── weather_dataset.csv
│── models/
│   ├── cart_model.pkl
│   ├── naive_bayes_model.pkl
│   └── cluster_model.pkl
│── src/
│   ├── preprocess.py
│   ├── train_models.py
│   ├── predict.py
│   └── utils.py
│── web/
│   ├── index.html
│   ├── styles.css
│   └── script.js
│── README.md
```

---

## 🚀 How to Run This Project

### **1. Clone the repository**

```bash
git clone https://github.com/yourusername/weather-prediction.git
cd weather-prediction
```

### **2. Install dependencies**

```bash
pip install -r requirements.txt
```

### **3. Train the models**

```bash
python src/train_models.py
```

### **4. Run the website**

Open the **web/index.html** in your browser.

---




