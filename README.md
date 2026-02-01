🚀 Student Performance Predictor (End-to-End ML Project)

A production-ready end-to-end Machine Learning application that predicts a student’s Maths score based on demographic and academic features.
The project covers the entire ML lifecycle — from data ingestion and model training to Dockerized deployment on Render.

🌐 Live Demo:👉 https://student-performance-predictor-ephw.onrender.com

📌 Problem Statement

Predict a student’s Maths score using:
Gender
Race / Ethnicity
Parental level of education
Lunch type
Test preparation course
Reading score
Writing score

This problem is treated as a regression task.

🧠 Solution Overview

The application follows industry-standard ML engineering practices:
Modular ML pipeline
Separate training and inference workflows
Serialized model & preprocessor artifacts
Flask-based web interface
Dockerized deployment
Cloud hosting on Render


⚙️ Tech Stack

Machine Learning
Python
Pandas
NumPy
Scikit-learn
CatBoost
XGBoost

🌐 Backend & Deployment

Flask
Gunicorn
Docker
Render (Cloud Hosting)

📊 Visualization & EDA

Matplotlib
Seaborn
Jupyter Notebook

🧩 ML Pipeline Details

1️⃣ Data Ingestion
Loads raw dataset
Splits into train/test sets
Saves intermediate artifacts

2️⃣ Data Transformation
Numerical & categorical preprocessing
ColumnTransformer
Saved as preprocessor.pkl

3️⃣ Model Training
Multiple models evaluated
Best model selected using R² score
Final model saved as model.pkl

4️⃣ Prediction Pipeline
Loads trained model & preprocessor
Validates input schema
Returns prediction to UI

🖥️ Web Application
User-friendly form UI
Real-time predictions
Error-safe inference pipeline
Same UI for local & production use

🐳 Dockerization
The entire application is containerized using Docker for:
Environment consistency
Easy deployment
Cloud portability
Build Image Locally
docker build -t student-performance-predictor .

Run Container
docker run -p 5000:5000 student-performance-predictor

☁️ Deployment (Render)
Docker-based Web Service
Automatic builds from GitHub
Free-tier hosting
Cold start supported

Live URL:
👉 https://student-performance-predictor-ephw.onrender.com 


