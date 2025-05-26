# 🩺 ML Project: Predicting Health Insurance Charges

This project builds a machine learning model to predict **health insurance charges** based on individual demographics and health factors. Alongside model development, it includes **data analysis reports** and a **Power BI dashboard** to provide end-to-end insights.

---

## 📌 Problem Statement

In the healthcare and insurance sector, predicting individual insurance charges is essential for:

- **Insurance companies** – accurate pricing, risk management, and customer segmentation  
- **Customers** – understanding premium breakdown and optimizing personal health decisions  
- **Policy makers** – creating data-driven policies  

The objective is to predict `charges in INR` using the following features:

- Age  
- Sex  
- BMI  
- Number of Children  
- Smoking Status  
- Region  
- BMI Category  
- Age Group  

---

## 📊 Exploratory Data Analysis (EDA)

Performed in both **Python** and **Excel** to extract insights:

- Distribution of charges by age and BMI categories  
- Impact of smoking on insurance charges  
- Average charges segmented by sex and region  
- Pivot tables and charts to summarize key relationships  

---

## 🧠 Machine Learning Workflow

### ✅ Step 1: Data Preparation
- Loaded data from `Machine_Learning_Dataset.xlsx`
- Dropped `Policy no.` as it’s an identifier
- Defined `charges in INR` as the target
- Feature separation: numerical and categorical

### ✅ Step 2: Preprocessing Pipeline
- Scaled numeric features using `StandardScaler`
- Encoded categorical features using `OneHotEncoder`
- Combined steps using `ColumnTransformer`

### ✅ Step 3: Model Building
- Algorithm used: **Random Forest Regressor**
- Hyperparameter tuning with `GridSearchCV` (5-fold CV)
- Built end-to-end pipeline for preprocessing + training

### ✅ Step 4: Model Evaluation

| Metric     | Value   |
|------------|---------|
| MAE        | 2530.88 |
| RMSE       | 4501.17 |
| R² Score   | 0.8695  |

### ✅ Step 5: Model Export
- Trained model saved as: `models/best_model.pkl`

---

## 📈 Dashboard and Reporting

A dedicated **Power BI Dashboard** and Excel reports were built to present findings in a visually interactive way.

**Power BI Dashboard Highlights:**
- Sales by Region
- Product/Service Performance
- Customer Segment Analysis
- Time-based Trends

**Reports Available:**
- Excel Report: Pivot analysis, charge trends
- Word Report: Written insights & business recommendations

---

## 💡 Technologies Used

| Category              | Tools / Libraries                        |
|-----------------------|------------------------------------------|
| Programming Language  | Python                                   |
| Data Manipulation     | pandas, numpy                            |
| Visualization         | Excel, Power BI                          |
| ML Algorithms         | Random Forest Regressor                  |
| Model Tuning          | GridSearchCV from scikit-learn           |
| Preprocessing         | StandardScaler, OneHotEncoder, Pipeline  |
| Model Export          | joblib                                   |
| Reporting             | Power BI, Excel Charts & Pivot Tables    |
| IDEs                  | Jupyter Notebook, VS Code                |

---

## 🗂️ Project Structure

Medibuddy-ML-Project/ <br>
│ <br>
├── data/<br>
│ └── Machine_Learning_Dataset.xlsx<br>
│<br>
├── dashboard/<br>
│ └── images<br>
│ └── Health Insurance Analytics Dashboard.pbix<br>
│<br>
├── notebook/<br>
│ └── model_building.ipynb<br>
│ └── predict.ipynb<br>
│<br>
├── models/<br>
│ └── best_model.pkl<br>
│<br>
├── reports/<br>
│ └── analysis_report.xlsx<br>
│ └── analysis_report.docx<br>
│<br>
├── README.md<br>
└── requirements.txt<br>

---

## ⚙️ How to Run the Project

1. **Clone the Repository**
git clone https://github.com/yourusername/ML-Project-predicting-health-insurance-charges-v2.git <br>
cd Medibuddy-ML-Project

2. **Install Dependencies**
pip install -r requirements.txt
3. **Open and Run the Notebook**
jupyter notebook notebook/model_building.ipynb

## 🔮 Future Scope
📊 Create an interactive Power BI dashboard <br>
🌐 Deploy model using Flask or Streamlit for real-time predictions <br>
📈 Try other models like XGBoost, SVR, Linear Regression <br>
⛏️ Perform advanced feature engineering <br>

## 👨‍💻 Author
Arnab Bandyopadhyay <br>
📧 arnab.bandyopadhyay01@gmail.com <br>
🔗 www.linkedin.com/in/arnab-bandyopadhyay-2a9269220

## 📄 License
This project is developed as part of an academic capstone and is meant for educational use only.
