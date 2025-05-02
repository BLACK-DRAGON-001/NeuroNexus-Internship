# 💳 Credit Card Fraud Detection — NeuroNexus Internship

## 📋 Project Overview

As part of the **NeuroNexus Internship**, this project focuses on building a machine learning model to detect **fraudulent credit card transactions**. With an emphasis on reducing false positives while maintaining high recall, the project tackles a **highly imbalanced dataset** using advanced data preprocessing, sampling techniques, and multiple classification models.

---

## 📚 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size:** 284,807 transactions
- **Fraudulent Class:** ~0.172% (highly imbalanced)
- **Features:**
  - `Time` and `Amount`
  - Principal Components (`V1` to `V28`)
  - `Class` (0 = genuine, 1 = fraud)

---

## ⚙️ Project Structure

📦 credit-card-fraud-detection/
├── data/ # Dataset files
├── notebooks/ # Jupyter Notebooks for EDA, preprocessing, and modeling
├── models/ # Trained model files (optional)
├── src/ # Modular Python scripts
├── requirements.txt # List of Python dependencies
├── LICENSE # Project license
└── README.md # Project overview and instructions


---

## 🚀 Implementation Pipeline

### 🔄 Data Preprocessing
- Checked for missing values (none found)
- Standardized `Time` and `Amount` features using `StandardScaler`

### 🧠 Feature Engineering
- Transaction frequency per user
- Merchant vs transaction location mismatch detection
- Spending pattern anomaly features

### ⚖️ Handling Class Imbalance
- **SMOTE:** Oversampling minority class
- **NearMiss:** Undersampling majority class
- Compared model performance with and without balancing

### 🧮 Model Training
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**

### 📊 Model Evaluation
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**
- **Confusion Matrix**

> Priority was given to **high recall** (to catch more frauds) while minimizing **false positives**.

---

## 🏆 Best Model

**Model:** Random Forest Classifier with SMOTE  
**Performance:**

| Metric        | Value    |
|---------------|----------|
| Accuracy      | 99.93%   |
| Precision     | 92.4%    |
| Recall        | 84.5%    |
| F1-Score      | 88.3%    |
| ROC-AUC Score | 98.9%    |

---

## 📈 Visualizations

- Class Distribution Plot
- Confusion Matrix Heatmap
- ROC-AUC Curve
- t-SNE Plot for dimensionality reduction

---

## 📋 Requirements

Make sure you have Python 3.8+ installed. Required libraries:

- `pandas`
- `numpy`
- `scikit-learn`
- `imbalanced-learn`
- `matplotlib`
- `seaborn`
- `tensorflow` 

Install dependencies:
```bash
pip install -r requirements.txt

🙌 Acknowledgements
Kaggle: Credit Card Fraud Detection Dataset

NeuroNexus Internship Program for mentorship and guidance

Community tutorials and academic resources on imbalanced classification

📬 Contact
Sarthak Dey
NeuroNexus Intern
📧 sarthakdbb@gmail.com 
🔗 GitHub: BLACK-DRAGON-001
