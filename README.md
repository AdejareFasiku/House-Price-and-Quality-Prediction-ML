# 🏠 House Price & Quality Prediction using Machine Learning

This project uses the **House Prices – Advanced Regression Techniques** dataset from Kaggle to build two predictive machine learning models:

1. **Regression Model** → Predicts the final sale price of a house  
2. **Classification Model** → Predicts the house’s overall quality category (Low, Medium, High)

The project demonstrates end-to-end machine learning workflows including data cleaning, exploration, feature engineering, modeling, and evaluation.

---

## 📌 Project Goals

### **1. Predict House Sale Price (Regression)**
- Models used:
  - Linear Regression  
  - Random Forest Regressor  
  - Gradient Boosting Regressor
- Evaluation Metric:
  - **RMSE (Root Mean Squared Error)**

### **2. Predict House Quality Category (Classification)**
- Categories:
  - **Low Quality** (1–4)
  - **Medium Quality** (5–7)
  - **High Quality** (8–10)
- Models used:
  - Logistic Regression  
  - Random Forest Classifier  
  - Gradient Boosting Classifier
- Evaluation Metrics:
  - **Accuracy**
  - **F1-Score**
  - **Confusion Matrix**

---

## 📂 Project Structure
House-Price-and-Quality-Prediction-ML/

│

├── data/

│ ├── train.csv
│ ├── test.csv
│ └── data_description.txt
│
├── notebooks_complete/
│ └── House_Prediction.ipynb.pdf # Full EDA + modeling notebook
│
├── House_Prediction.ipynb
├── README.md
└── requirements.txt


---

## 🧹 Data Preprocessing

Key steps included:

- Handling missing values (median for numeric, "None" for categorical)
- Encoding categorical variables using **One-Hot Encoding**
- Scaling features when required (for linear models)
- Feature engineering:
  - `TotalSF` (Total Square Footage)
  - `TotalBathrooms`
  - `YearsSinceRemodel`
  - `HouseAge`
  - `TotalPorchSF`
  - Boolean flags: `HasPool`, `HasFireplace`, `HasGarage`

---

## 📊 Exploratory Data Analysis

EDA included:

- Distribution plots for key numeric features  
- Correlation heatmap of all numeric variables  
- Boxplots comparing quality vs sale price  
- Missing value visualization  
- Neighborhood-level price trends  

Visual insights guided feature engineering and model selection.

---

## 🤖 Machine Learning Models

### **Regression Models**
- Linear Regression  
- Random Forest Regressor  
- Gradient Boosting Regressor

### **Classification Models**
- Logistic Regression  
- Random Forest Classifier  
- Gradient Boosting Classifier

Models were trained, validated, and evaluated using:
- **Train/Test Split**
- **Cross-Validation**
- **Hyperparameter Tuning** (where applicable)

---

## 📈 Results Summary

### **Regression**
- Gradient Boosting Regressor achieved the best performance  
- RMSE significantly improved after feature engineering  

### **Classification**
- Random Forest Classifier achieved the highest accuracy and macro F1-score  
- Confusion matrix showed good separation between categories  

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **Scikit-Learn**
- **Jupyter Notebook**

---

## 📥 Dataset Source

This project uses the public dataset from Kaggle:

🔗 *House Prices – Advanced Regression Techniques*  
https://www.kaggle.com/c/house-prices-advanced-regression-techniques

---

## 🚀 How to Run the Project

### 1. Clone the repository:
```bash
git clone https://github.com/AdejareFasiku/House-Price-and-Quality-Prediction-ML.git
cd <House-Price-and-Quality-Prediction-ML>
