📌 Project Overview
A machine learning-based system designed to detect early signs of mental health issues among students. This project analyzes survey data to categorize mental health states and provide insights, serving as a tool for early identification and supportive intervention in educational institutions.

Done By:

P. Himani (22MIC7207)

B. Venkata Sai Keerthana (22MIC7127)

M. Harshavardhini (22MIC7015)

Faculty Advisor: B. Mohinder Singh

🎯 Problem Statement
Mental health issues among students are increasing due to academic pressure, social challenges, and personal struggles. Lack of early detection can lead to serious consequences like depression, anxiety, and dropouts. This project provides a technological solution to assist in early identification.

✨ Features
Predictive Analysis: ML models to detect mental health issues from survey data

Multi-Class Classification: Categorizes mental health state into Normal, Mild, Moderate, or Severe

Data Insights: Identifies key factors affecting student mental health

User-Friendly Interface: Accessible platform for interaction and results display

🛠️ Tech Stack
Programming Language: Python

ML Libraries: Pandas, NumPy, Scikit-learn, Matplotlib

Development Environment: Google Colab

Deployment: Render (Backend), GitHub (Version Control)

App Development: MIT App Inventor (for potential mobile interface)

📊 Dataset
The project uses datasets from Kaggle containing student mental health surveys with various parameters such as:

Academic pressure levels

Sleep patterns

Social connectedness

Extracurricular activities

Personal demographics

📁 Project Structure
text
student-mental-health-using-ml/
│
├── copy_of_student_mentalhealth_andysing.py  # Main ML implementation
├── requirements.txt                           # Project dependencies
├── copy_of_student_mentalhealth_analysis.py                                    # Flask API (if applicable)
├── mental_health_dataset.csv                  # Dataset (or reference)
└── README.md                                  # Project documentation
🚀 Installation & Setup
Prerequisites
Python 3.8+

pip (Python package manager)

Local Installation
Clone the repository

bash
git clone https://github.com/YourUsername/student-mental-health-using-ml.git
cd student-mental-health-using-ml
Create a virtual environment (recommended)

bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies

bash
pip install -r requirements.txt
Run the application

bash
python copy_of_student_mentalhealth_andysing.py
📋 API Documentation (If Applicable)
If you have implemented a Flask API, include this section:

Prediction Endpoint
POST /predict

Request Body:

json
{
  "academic_pressure": 8,
  "sleep_hours": 5,
  "social_connectedness": 3,
  "extracurricular_hours": 2,
  "study_hours": 6
}
Response:

json
{
  "prediction": "Moderate",
  "confidence": 0.78,
  "risk_factors": ["sleep_hours", "academic_pressure"]
}
Example using curl
bash
curl -X POST https://your-app-name.onrender.com/predict \
  -H "Content-Type: application/json" \
  -d '{"academic_pressure": 8, "sleep_hours": 5, "social_connectedness": 3, "extracurricular_hours": 2, "study_hours": 6}'
🧠 Machine Learning Models
The project implements and compares various classification algorithms:

Logistic Regression

Support Vector Machines (SVM)

Decision Trees

Random Forest

📈 Results
Our models achieve 70-90% accuracy in predicting mental health states, consistent with findings from literature review. Key factors identified include academic pressure, sleep patterns, and social connectedness.

🌐 Deployment
The application is deployed on Render:

Live Demo: https://your-app-name.onrender.com

Build Command: pip install -r requirements.txt

Start Command: gunicorn app:app (for Flask API)

👥 Contributors
P. Himani (22MIC7207) - ML Model Development

B. Venkata Sai Keerthana (22MIC7127) - Data Preprocessing & Analysis

M. Harshavardhini (22MIC7015) - UI/App Development & Deployment

📄 License
This project is created for academic purposes as part of the summer project.

🤝 Acknowledgments
Faculty Advisor B. Mohinder Singh for guidance

Kaggle for providing relevant datasets

Render for deployment platform
