# 🫀 Heart Disease Predictor

A Machine Learning-based web application that predicts the likelihood of heart disease from user health data.  
This project combines Python, Flask, and Scikit-Learn to build an ML model and expose it through a backend API, with visualizations and ROC curve support.

Website images:
<img width="1920" height="1080" alt="Screenshot (143)" src="https://github.com/user-attachments/assets/e93f79fb-13ab-46a9-ad79-d7793ad21cef" />

<img width="1920" height="1080" alt="Screenshot (144)" src="https://github.com/user-attachments/assets/772602f3-f605-411b-9660-b53fb6f2420a" />

<img width="1920" height="1080" alt="Screenshot (145)" src="https://github.com/user-attachments/assets/db81f44f-9efa-4cd5-b7e1-15a967cf304f" />

<img width="1920" height="1080" alt="Screenshot (146)" src="https://github.com/user-attachments/assets/325ca1d9-479d-41d2-87c4-d507e82cab17" />

<img width="1920" height="1080" alt="Screenshot (147)" src="https://github.com/user-attachments/assets/5f481fae-0a0d-4d02-9d9e-215ebe736f34" />

<img width="1920" height="1080" alt="Screenshot (148)" src="https://github.com/user-attachments/assets/a5ed6592-8e73-4891-9c09-b3f1ac9ee7e2" />

<img width="1920" height="1080" alt="Screenshot (149)" src="https://github.com/user-attachments/assets/0fe465f1-9c71-485c-863f-a4842b82c54f" />

<img width="1920" height="1080" alt="Screenshot (150)" src="https://github.com/user-attachments/assets/c835dc2d-baae-4cd0-bdc9-ad18935e6cdf" />

<img width="1920" height="1080" alt="Screenshot (151)" src="https://github.com/user-attachments/assets/9b9deed9-91f5-467f-b5ba-694a818e4767" />

<img width="1920" height="1080" alt="Screenshot (152)" src="https://github.com/user-attachments/assets/e30dd9b7-7c00-4086-82c9-013ebcb7fcc2" />

<img width="1920" height="1080" alt="Screenshot (153)" src="https://github.com/user-attachments/assets/14cb110d-3331-4a50-844a-831701f85d9f" />

<img width="1920" height="1080" alt="Screenshot (155)" src="https://github.com/user-attachments/assets/a5f8ae28-b7a2-4be8-a242-e3432a0f882b" />



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









