# 🩺 ML Project: Predicting Health Insurance Charges 

The goal of this project is to build a predictive machine learning model that estimates **health insurance charges** based on user demographics and lifestyle features.

In addition to model building, extensive **Exploratory Data Analysis (EDA)** and visual reporting have been done to understand cost-driving factors. The model helps forecast costs, optimize pricing, and guide policy decisions.

---

## 📌 Problem Statement

The healthcare and insurance industry needs a reliable way to **predict medical insurance costs**. Accurate cost prediction helps:

- Insurance companies in premium setting and customer segmentation  
- Customers understand the factors affecting their premium  
- To enhance personalization in its service offerings  

We aim to build a machine learning model to predict `charges in INR` using features such as:

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

Before building the model, we conducted a thorough EDA using **Excel** and **Python**, which included:

- Distribution of charges across age groups and BMI categories  
- Relationship between smoking habits and costs  
- Average charges per region and sex  

## 🧠 Machine Learning Workflow

### ✅ Step 1: Data Preparation
- Loaded dataset from `Machine_Learning_Dataset.xlsx`  
- Dropped `Policy no.` (an identifier)  
- Defined `charges in INR` as the target variable  
- Separated numerical and categorical features  

### ✅ Step 2: Preprocessing Pipeline
- Used `StandardScaler` for numerical features  
- Used `OneHotEncoder` for categorical features  
- Built a preprocessing pipeline using `ColumnTransformer`  

### ✅ Step 3: Model Building
- Algorithm: **Random Forest Regressor**  
- Tuned hyperparameters using `GridSearchCV` with 5-fold cross-validation  
- Pipeline included both preprocessing and model training  

### ✅ Step 4: Model Evaluation

| Metric     | Value       |
|------------|-------------|
| MAE        | 2530.88     |
| RMSE       | 4501.17     |
| R² Score   | 0.8695      |

### ✅ Step 5: Model Export
- Saved trained model as a `.pkl` file using `joblib`
- location: /models/best_model.pkl 

---

## 💡 Technologies Used

| Category              | Tools / Libraries                       |
|-----------------------|------------------------------------------|
| Programming Language  | Python                                   |
| Data Manipulation     | pandas, numpy                            |
| Visualization         | seaborn, matplotlib, Excel               |
| ML Algorithms         | Random Forest Regressor                  |
| Model Tuning          | GridSearchCV from scikit-learn           |
| Preprocessing         | StandardScaler, OneHotEncoder, Pipeline  |
| Model Export          | joblib                                   |
| Reporting             | Excel Charts and Pivot Tables            |
| IDEs                  | Jupyter Notebook, VS Code                |

---

## 🗂️ Project Structure

Medibuddy-ML-Project/ <br>
│ <br>
├── data/<br>
│ └── Machine_Learning_Dataset.xlsx<br>
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
📊 Create an interactive Power BI dashboard
🌐 Deploy model using Flask or Streamlit for real-time predictions
📈 Try other models like XGBoost, SVR, Linear Regression
⛏️ Perform advanced feature engineering

## 👨‍💻 Author
Arnab Bandyopadhyay
📧 arnab.bandyopadhyay01@gmail.com
🔗 www.linkedin.com/in/arnab-bandyopadhyay-2a9269220

## 📄 License
This project is developed as part of an academic capstone and is meant for educational use only.
