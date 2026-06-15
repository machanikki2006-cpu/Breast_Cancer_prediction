# Breast Cancer Prediction Model

A Machine Learning project for predicting breast cancer diagnosis using classification algorithms. This model uses the **Breast Cancer dataset** to classify tumors as **Malignant (M)** or **Benign (B)** using **Logistic Regression** and **Support Vector Machine (SVM)**.

## 📌 Project Overview

The goal of this project is to build a machine learning model that predicts whether a breast tumor is malignant or benign based on medical features.

The project includes:

- Data preprocessing
- Feature scaling
- Model training
- Hyperparameter tuning
- Model evaluation

Two machine learning models were implemented and compared:

1. **Logistic Regression**
2. **Support Vector Machine (SVM)**

---

## 📂 Dataset

The dataset used is the **Breast Cancer Dataset** containing tumor-related features.

### Features include:
- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Symmetry
- Fractal dimension
- And more...

### Target Variable
- **M** → Malignant (Cancerous)
- **B** → Benign (Non-cancerous)

---

## ⚙️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Scikit-learn**

---

## 🛠️ Project Workflow

### 1. Data Preprocessing
- Loaded the dataset using Pandas
- Removed unnecessary columns (`id`)
- Checked for:
  - Missing values
  - Duplicate data
- Converted categorical diagnosis labels into numerical format using `get_dummies()`

### 2. Feature Engineering
- Split features (`X`) and target (`y`)
- Applied **StandardScaler** for feature normalization

### 3. Train-Test Split
- Dataset split into:
  - **70% Training**
  - **30% Testing**

### 4. Model Training

#### Logistic Regression
- Used:
```python
LogisticRegression(class_weight='balanced')
```

#### Support Vector Machine (SVM)
- Hyperparameter tuning performed using **GridSearchCV**
- Parameters tuned:
  - `C`
  - `kernel`
  - `gamma`

---

## 📊 Model Evaluation

The models were evaluated using:

- **Precision Score**
- **Recall Score**
- **F1 Score**
- **Confusion Matrix**
- **Classification Report**

### Logistic Regression Performance
Achieved high performance with strong precision, recall, and F1-score.

### SVM Performance
Optimized using Grid Search and produced highly accurate predictions.

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/cancer-prediction-model.git
```


---
