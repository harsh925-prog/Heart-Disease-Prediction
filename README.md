# ❤️ Heart Disease Prediction using Logistic Regression

This project is a **Machine Learning web application** built with **Streamlit** that predicts the **risk of heart disease** based on clinical and lifestyle parameters entered by the user.

The model uses **Logistic Regression** for binary classification and achieves an accuracy of **87.5%** on the test dataset.

---

## 🚀 Live Demo
👉 https://heart-disease-prediction-trs56pdvcaceughdshbquu.streamlit.app/

---

## 📌 Project Overview

Heart disease is one of the leading causes of death worldwide. Early detection plays a critical role in preventing severe health outcomes.  
This application helps estimate the **likelihood of heart disease** using patient medical data through an easy-to-use web interface.

This project is intended for **educational and demonstration purposes**.

---

## 🧠 Machine Learning Model

- **Algorithm**: Logistic Regression  
- **Problem Type**: Binary Classification  
- **Accuracy**: **87.5%**  
- **Preprocessing Techniques**:
  - One-hot encoding for categorical variables
  - Feature scaling using a trained scaler
  - Consistent feature ordering using saved column metadata

---

## 🗂️ Project Structure

heart-disease-prediction/
│
├── app.py
├── model.pkl
├── scaler.pkl
├── columns.pkl
├── requirements.txt
├── README.md
└── screenshots/
├── home.png
└── prediction.png

yaml
Copy code

---

## 🧪 Input Features

- Age  
- Sex (M / F)  
- Chest Pain Type (ATA, NAP, TA, ASY)  
- Resting Blood Pressure (mm Hg)  
- Cholesterol (mg/dL)  
- Fasting Blood Sugar (0 or 1)  
- Resting ECG (Normal, ST, LVH)  
- Maximum Heart Rate  
- Exercise-Induced Angina (Y / N)  
- Oldpeak (ST Depression)  
- ST Slope (Up, Flat, Down)

Categorical features are automatically **one-hot encoded** inside the application.

---

## ⚙️ How the Application Works

1. User enters medical details through the Streamlit interface  
2. Inputs are converted to the expected feature format  
3. Missing columns are added using `columns.pkl`  
4. Data is scaled using `scaler.pkl`  
5. Logistic Regression model predicts the result  
6. Output is displayed as:
   - **High Risk of Heart Disease**
   - **Low Risk of Heart Disease**

---

## 📸 Application Screenshots

### Input Form
![Input Form](screenshots/home.png)

### Prediction Result
![Prediction Result](screenshots/prediction.png)

---

## ▶️ Run the Application Locally

```bash
git clone https://github.com/harsh925-prog/Heart-Disease-Prediction.git
cd Heart-Disease-Prediction
pip install -r requirements.txt
streamlit run app.py
☁️ Deployment
The application is deployed using Streamlit Community Cloud.

Platform: Streamlit Community Cloud

Source Control: GitHub

Deployment Type: Public Web App

Auto-redeploy on GitHub push: Enabled

⚠️ Disclaimer
This project is for educational purposes only and should not be used for medical diagnosis.