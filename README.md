# 🫀 Heart Disease Predictor

A Machine Learning-based web application that predicts the likelihood of heart disease from user health data.  
This project combines Python, Flask, and Scikit-Learn to build an ML model and expose it through a backend API, with visualizations and ROC curve support.

---

## 📌 Project Overview

Heart disease is one of the **leading causes of death worldwide**. Early detection can significantly improve prognosis. This project uses a trained machine learning model to estimate a patient’s risk of heart disease based on clinical health parameters.

It takes input like age, blood pressure, cholesterol, etc., and returns a **probability of heart disease**, helping healthcare professionals or users identify potential risk. :contentReference[oaicite:1]{index=1}

---

## 🧠 Features

✔ Predicts the likelihood of heart disease using clinical data  
✔ REST API built with **Flask**  
✔ Trained model using **scikit-learn**  
✔ Visual performance analysis (ROC Curve)  
✔ Modular Python Flask backend structure  

---

## 📂 Repository Structure
Heart_disease_predictor/
├── app/ # Flask app package
│ ├── routes.py # Route definitions for API
│ └── init.py # Flask application factory
├── data/ # Dataset for training/testing (if any)
├── requirements.txt # Required dependencies
├── run.py # Application entry point
├── roc curve.png # ROC performance visualization
└── README.md # Project documentation

## 🛠️ Tech Stack
| Layer | Technology |
|------|------------|
| Backend | Python, Flask |
| Machine Learning | scikit-learn |
| Data Handling | NumPy, pandas |
| Visualization | Chart.js / Matplotlib |
| Model Serialization | joblib |

Dependencies are listed in `requirements.txt`:  
Flask
joblib
numpy
pandas
scikit-learn
chart.js

## 🧾 Installation

**1. Clone the repository**
```bash
git clone https://github.com/Eshwari-coder-sys/Heart_disease_predictor.git
cd Heart_disease_predictor
2. Create virtual environment (recommended)
python -m venv .venv
3. Activate venv
Windows:
.\.venv\Scripts\activate
4. Install dependencies
pip install -r requirements.txt

🚀 Running the Application
Start the Flask server: python run.py

API Endpoints (Example)
POST /predict

Send JSON payload like:
{
  "age": 55,
  "sex": 1,
  "cholesterol": 240,
  "rest_blood_pressure": 130,
  …
}

Returns:
{
  "prediction": 1,
  "risk_score": 0.82
}

Meaning: High risk of heart disease

Model Performance:
A ROC curve image (roc curve.png) is included to show classification performance.
Model evaluates True Positive vs. False Positive rate
Helps visualize classification quality
(ROC is common for binary classification in health prediction problems.)

📈 Future Improvements:
✔ Add Frontend UI (React / Streamlit)
✔ Add user authentication & dashboards
✔ Improve model using feature engineering and cross-validation
✔ Save models using more robust methods (e.g., Pickle, ONNX)
