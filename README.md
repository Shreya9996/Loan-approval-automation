# Loan-approval-automation


# 🏦 AI-Powered Loan Approval System

<p align="center">
<img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/n8n-Workflow-EA4B71?style=for-the-badge&logo=n8n&logoColor=white"/>
<img src="https://img.shields.io/badge/Automation-AI-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/License-MIT-success?style=for-the-badge"/>
</p>

<h1 align="center">
🤖 AI-Powered Loan Approval System
</h1>

<p align="center">
AI-powered Loan Approval System using KNN, FastAPI, and n8n for automated loan prediction, PDF report generation, and email notifications.
</p>

---

# 📌 Overview

Traditional loan approval processes are often manual, time-consuming, and prone to inconsistencies. This project leverages Machine Learning and workflow automation to streamline the process.

The application predicts whether a loan should be **Approved** or **Rejected**, generates a professional PDF decision report, and automatically emails the report to the applicant.

---

# ✨ Features

* 🤖 AI-based Loan Approval Prediction
* 📊 Machine Learning (KNN Classifier)
* ⚡ FastAPI REST API
* 🔄 End-to-End Automation using n8n
* 📄 Automatic PDF Report Generation
* 📧 Email Notification with PDF Attachment
* 📈 Real-time Prediction Results
* 📝 Clean and Modular Architecture

---

# 🏗️ System Architecture

```text
                 Applicant
                     │
                     ▼
          Loan Application Form
                     │
                     ▼
                FastAPI Backend
                     │
                     ▼
          Machine Learning Model
              (KNN Classifier)
                     │
         ┌───────────┴───────────┐
         │                       │
         ▼                       ▼
   Loan Approved          Loan Rejected
         │                       │
         └───────────┬───────────┘
                     ▼
          Generate PDF Report
                     │
                     ▼
              n8n Workflow
                     │
                     ▼
          Email with PDF Report
                     │
                     ▼
                 Applicant
```

---

# 🧠 Machine Learning Model

The prediction engine is based on the **K-Nearest Neighbors (KNN)** algorithm.

### Workflow

```text
Applicant Data
       │
       ▼
Data Preprocessing
       │
       ▼
Feature Scaling
       │
       ▼
KNN Model
       │
       ▼
Prediction
       │
       ▼
Approved / Rejected
```

---

# 🛠️ Technology Stack

| Category             | Technology       |
| -------------------- | ---------------- |
| Programming Language | Python           |
| Machine Learning     | Scikit-learn     |
| Backend API          | FastAPI          |
| Workflow Automation  | n8n              |
| Data Processing      | Pandas, NumPy    |
| Model Development    | Google Colab     |
| Report Generation    | ReportLab / FPDF |
| Email Service        | SMTP (via n8n)   |

---

# 📂 Project Structure

```text
Loan-Approval-System/
│
├── app/
│   ├── main.py
│   ├── predict.py
│   └── utils.py
│
├── model/
│   ├── loan_model.pkl
│   └── scaler.pkl
│
├── dataset/
│
├── notebooks/
│   └── Loan_Model_Training.ipynb
│
├── reports/
│
├── workflow/
│   └── n8n-workflow.json
│
├── screenshots/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

# 🔄 Workflow

### Step 1

Applicant submits loan information.

⬇️

### Step 2

FastAPI receives the request.

⬇️

### Step 3

The trained KNN model predicts loan eligibility.

⬇️

### Step 4

A PDF report is generated automatically.

⬇️

### Step 5

n8n sends the PDF report via email.

---

# 📊 Model Performance

| Metric     | Value                 |
| ---------- | --------------------- |
| Algorithm  | KNN                   |
| Accuracy   | **90%**               |
| Prediction | Binary Classification |

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/loan-approval-system.git
```

Go to project folder

```bash
cd loan-approval-system
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run FastAPI

```bash
uvicorn app.main:app --reload
```

Open API Documentation

```text
http://127.0.0.1:8000/docs
```

---

# 📧 n8n Automation

The workflow automatically:

* Receives prediction results
* Generates a PDF report
* Attaches the PDF
* Sends an email to the applicant
* Stores workflow logs

---

# 📸 Screenshots

Add screenshots in the **screenshots/** folder.

Example:

* Home Page
* FastAPI Swagger UI
* Loan Prediction Output
* n8n Workflow
* Generated PDF
* Email Received

---

# 📈 Future Enhancements

* Random Forest & XGBoost Models
* Explainable AI (SHAP/LIME)
* Streamlit Dashboard
* Docker Deployment
* Cloud Deployment
* Database Integration
* User Authentication
* Admin Dashboard

---

# 🎯 Project Objectives

✔ Reduce manual loan approval time

✔ Improve prediction accuracy

✔ Automate repetitive tasks

✔ Generate professional decision reports

✔ Improve applicant communication

---

# 🤝 Contributing

Contributions are welcome!

1. Fork this repository
2. Create a new branch
3. Commit your changes
4. Open a Pull Request

---

# 📜 License

This project is licensed under the **MIT License**.

---

# 👩‍💻 Author

### **Shreya Patil**

🎓 Computer Science Engineering Student

💻 Machine Learning | Deep Learning | Data Science

🚀 FastAPI • n8n • Python • Scikit-learn

⭐ If you found this project helpful, don't forget to **Star ⭐ this repository!**
