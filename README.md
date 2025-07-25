# 💼 Employee Salary Predictor - Farman Malik

This project predicts employee salary classes using a machine learning classification model trained on structured demographic and employment data. It features an end-to-end pipeline—from data preprocessing and model training to web deployment using Streamlit and ngrok.

---

##  Project Overview

- **Objective**: To build a machine learning model that predicts the salary class of an employee based on features like age, workclass, marital status, gender, occupation, and native country.
- **Algorithm Used**: Gradient Boosting Classifier
- **Deployment**: Web-based interface using Streamlit and shared publicly via ngrok/Grok

---

##  Features Used for Prediction

- Age  
- Workclass  
- Marital Status  
- Gender  
- Occupation  
- Native Country

These features were preprocessed and encoded appropriately before being fed into the classifier.

---

## 🛠️ Technologies & Tools

| Task                        | Technology       |
|-----------------------------|------------------|
| Data Cleaning & EDA         | Pandas, NumPy     |
| Visualization               | Matplotlib, Seaborn |
| Model Training              | Scikit-learn      |
| Serialization               | Joblib           |
| Web Application             | Streamlit         |
| Deployment                  | ngrok / Grok      |
| Notebook Environment        | Google Colab      |

---

## 🧪 Model Training Workflow

1. **Data Preprocessing**:
   - Removed missing values and outliers
   - Label encoding of categorical columns
   - Feature reduction: Dropped low-impact columns like 'education'
2. **Model Training**:
   - Tried multiple classifiers: Logistic Regression, Random Forest, XGBoost
   - Final model: **Gradient Boosting Classifier** (achieved highest accuracy)
3. **Evaluation**:
   - Accuracy, Precision, Recall, F1-score
   - Confusion matrix visualization

---

## 🌐 Streamlit Web App Integration

- Created a lightweight Streamlit dashboard (`app.py`)
- Users can enter input fields and get real-time salary class predictions
- Hosted and tunneled publicly using `ngrok` or Grok CLI

### 🔗 Public Deployment (via ngrok)
```bash
!pip install streamlit pyngrok
!streamlit run app.py &
!ngrok authtoken <30C4SLgYjt6YBsSm4KZZou4DSp0_7UseLVsvHki5cUVaJb6eZ>
!ngrok http 8501
