❤️ Heart Disease Prediction using Logistic Regression

This project is a **Machine Learning web application** built with **Streamlit** that predicts the **risk of heart disease** based on clinical and lifestyle parameters entered by the user.

The model uses **Logistic Regression** for binary classification and achieves an accuracy of **87.5%** on the test dataset.

---

🚀 Live Demo
👉 Add your Streamlit Cloud URL here after deployment

---

📌 Project Overview

Heart disease is one of the leading causes of death worldwide. Early detection plays a critical role in preventing severe health outcomes.  
This application helps estimate the **likelihood of heart disease** using patient medical data through an easy-to-use web interface.

This project is intended for **educational and demonstration purposes**.

---

🧠 Machine Learning Model

- **Algorithm**: Logistic Regression  
- **Problem Type**: Binary Classification  
- **Accuracy**: **87.5%**  
- **Preprocessing Techniques**:
  - One-hot encoding for categorical variables
  - Feature scaling using a trained scaler
  - Consistent feature ordering using saved column metadata

---

🗂️ Project Structure

heart-disease-prediction/
│
├── app.py # Streamlit web application
├── model.pkl # Trained Logistic Regression model
├── scaler.pkl # Feature scaler used during training
├── columns.pkl # Expected feature order
├── requirements.txt # Required Python packages
└── README.md # Project documentation


---

🧪 Input Features

The following medical parameters are used for prediction:

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

⚙️ How the Application Works

1. User enters health-related details via the Streamlit interface  
2. Inputs are transformed to match the training feature format  
3. Missing columns are added using stored metadata  
4. Data is scaled using the saved scaler  
5. Logistic Regression model predicts the result  
6. Output is displayed as:
   - **High Risk of Heart Disease**
   - **Low Risk of Heart Disease**

---

▶️ Run the Application Locally

Step 1: Clone the repository
```bash
git clone https://github.com/your-username/heart-disease-prediction.git
cd heart-disease-prediction

Step 2: Install dependencies
pip install -r requirements.txt

Step 3: Start the Streamlit app
streamlit run app.py