#  RaktCare AI – Intelligent Blood Donation Management System

## Overview

**RaktCare AI** is an AI-powered blood donation management platform designed to streamline the process of connecting blood donors with hospitals and patients. By leveraging Machine Learning, predictive analytics, and Generative AI, the system helps healthcare organizations identify the most suitable donors, forecast blood shortages, and improve emergency response times.

Unlike traditional blood bank management systems that rely on manual donor searches, RaktCare AI uses predictive models to prioritize donors based on their likelihood of donating, donation history, and eligibility.

---

## Problem Statement

Blood banks and hospitals often face challenges such as:

* Difficulty identifying available donors during emergencies.
* Time-consuming manual donor outreach.
* Lack of prediction for future blood shortages.
* Inefficient donor prioritization.
* Limited access to accurate blood donation information.

RaktCare AI addresses these challenges through AI-driven decision-making and automation.

---

# Key Features

### 🩸 Donor Registration & Management

* Secure donor profile creation and management.
* Maintains donor information, blood group, medical eligibility, and donation history.

### 🤖 Donor Availability Prediction

* Predicts the probability that a donor will be available for donation.
* Uses historical donation behavior and donor attributes.
* Helps hospitals contact the most promising donors first.

### 📈 Donation Frequency Prediction

* Estimates when a donor is likely to donate again.
* Supports long-term donor engagement and campaign planning.

### 📊 Blood Shortage Forecasting

* Forecasts potential shortages for different blood groups.
* Enables proactive blood donation drives before shortages occur.

### 🩸 Blood Compatibility Engine

* Automatically identifies compatible donors based on blood group compatibility rules.
* Reduces manual filtering during emergencies.

### 🏆 Intelligent Donor Ranking

* Ranks donors using multiple factors such as:

  * Availability
  * Donation history
  * Eligibility
  * Location (if applicable)
  * Predicted response probability

### 💬 AI Assistant

* Integrated Gemini AI assistant for answering blood donation and healthcare-related queries.
* Provides instant guidance to donors and users.

---

# System Architecture

```
                User
                  │
          React Frontend
                  │
             REST API
                  │
           FastAPI Backend
      ┌─────────┼─────────┐
      │         │         │
 ML Models   Gemini AI   Database
      │
 Predictions & Analytics
```

---

# Technology Stack

## Frontend

* React.js
* HTML5
* CSS3
* JavaScript

## Backend

* FastAPI
* Python

## Machine Learning

* Scikit-learn
* XGBoost
* Pandas
* NumPy

## Database

* SQL Database

## AI Integration

* Google Gemini API

---

# Machine Learning Pipeline

1. Data Collection
2. Data Cleaning & Preprocessing
3. Feature Engineering
4. Model Training
5. Model Evaluation
6. Model Serialization
7. FastAPI Model Deployment
8. Real-time Predictions

---

# ML Models

## 1. Donor Availability Prediction

**Objective:** Predict whether a donor is likely to donate when contacted.

**Algorithm**

* XGBoost Classifier

**Evaluation Metrics**

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

---

## 2. Donation Frequency Prediction

**Objective**
Estimate the time until the donor's next donation.

**Algorithm**

* Regression Model

**Evaluation Metric**

* R² Score

---

## 3. Blood Shortage Forecasting

Uses historical donation trends and demand patterns to forecast shortages for different blood groups.

---

# Project Workflow

```
User Registration
        │
        ▼
Store Donor Information
        │
        ▼
Hospital Requests Blood
        │
        ▼
Retrieve Eligible Donors
        │
        ▼
Availability Prediction
        │
        ▼
Donation Frequency Prediction
        │
        ▼
Compatibility Check
        │
        ▼
Donor Ranking
        │
        ▼
Recommended Donor List
```

---

# Folder Structure

```
RaktCare-AI/
│
├── frontend/              # React application
├── backend/               # FastAPI backend
├── models/                # Trained ML models
├── datasets/              # Dataset used for training
├── notebooks/             # Model development notebooks
├── utils/                 # Helper functions
├── api/                   # API routes
├── requirements.txt
└── README.md
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/raktcareAI.git
cd raktcareAI
```

## Create Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Backend

```bash
uvicorn app:app --reload
```

## Run Frontend

```bash
npm install
npm start
```

---

# Future Enhancements

* Real-time donor location tracking.
* SMS and email notifications.
* Mobile application.
* Cloud deployment.
* Explainable AI for prediction transparency.
* Continuous model retraining with new donor data.
* Hospital analytics dashboard.

---

# Impact

RaktCare AI aims to improve emergency blood donation management by:

* Reducing donor search time.
* Increasing donor response rates.
* Improving hospital decision-making.
* Forecasting blood shortages.
* Enhancing healthcare accessibility using Artificial Intelligence.

---

# Contributors

This project was developed to demonstrate the application of Artificial Intelligence, Machine Learning, and Full-Stack Development in solving real-world healthcare challenges. Contributions and suggestions are welcome to further improve the platform.

---

# License

This project is intended for educational and research purposes. Please ensure compliance with applicable data privacy regulations and ethical guidelines before deploying it in a production healthcare environment.
