# Healthcare Appointment No-Show Prediction & Operational Analytics

## Overview
Machine learning–powered operational analytics solution that predicts patient no-shows, identifies key drivers, and provides actionable insights to improve scheduling efficiency and reduce wasted clinical capacity.

## Problem Statement
Healthcare organizations lose time, resources, and revenue due to high appointment no-show rates. Traditional reporting does not reveal the underlying behavioral or demographic patterns.

## Objectives
- Build ML classification model to predict no-show likelihood.
- Provide operational KPIs for clinics and physicians.
- Visualize patient behavior patterns using Tableau.
- Recommend interventions to reduce no-shows.

## Dataset
- Kaggle: Medical Appointment No-Show Dataset  

## ML Algorithms Used
- Logistic Regression  
- Random Forest  
- XGBoost / LightGBM  
- SVM  
- SMOTE (for imbalance)  
- SHAP for model explainability  

## Tools & Technologies
- Python (Pandas, Scikit-Learn, XGBoost, SHAP)
- PySpark (optional variant for big data)
- Tableau (dashboard)
- Streamlit (interactive ML prediction UI)
- FastAPI + Docker (optional deployment)

## Key Steps
1. Clean and preprocess patient & appointment data.
2. Perform EDA (demographics, waiting time, health indicators).
3. Engineer features (SMS reminders, clinic distance).
4. Train ML models; evaluate AUC, precision, recall.
5. Build Tableau visual dashboards for clinic operations.
6. Deploy model as a Streamlit app (optional).

## Insights
- Identified key patient behaviors affecting attendance.  
- Built explainable ML model with actionable recommendations.  

## Folder Structure
- `/dashboards` – Tableau files / images  
- `/notebooks` – ML notebooks  
- `/sql` – preprocessing scripts  
- `/images` – visuals  

