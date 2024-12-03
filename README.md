# Predictive-maintainance-using-ML


This project focuses on **predictive maintenance** of industrial machines using various machine learning models. The goal is to predict machine failures based on historical data and features such as temperature, rotational speed, and torque. The project also includes a **Streamlit application** for a user-friendly interface to classify whether a machine will fail.

---


---

## Overview

Predictive maintenance is crucial in minimizing downtime and maintenance costs. This project implements machine learning models like Logistic Regression, Decision Tree, Random Forest, and SVM to predict machine failures based on features such as:

- Air temperature
- Process temperature
- Rotational speed
- Torque

The best-performing model, **Random Forest**, is saved and deployed for prediction using a Streamlit web application.

---

## Dataset

The dataset used for this project is `predictive_maintenance.csv`. It contains features such as:

- **Type**: The category of the machine (`L`, `M`, or `H`).
- **Air temperature [K]**
- **Process temperature [K]**
- **Rotational speed [rpm]**
- **Torque [Nm]**
- **Tool wear [min]**
- **Target**: Indicator of failure (0 = No Failure, 1 = Failure).

---

## Machine Learning Models

The following models were trained and evaluated:

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest** (Best performer)
4. **Support Vector Machine (SVM)**

Performance of the models was evaluated using:
- Training accuracy
- Test accuracy
- Classification report
- Confusion matrix

---

## Streamlit Application

A **Streamlit application** is included to provide a simple and intuitive user interface for predicting whether a machine will fail. Users can input feature values such as temperature, speed, and torque, and the model outputs whether the machine will fail or not.

### Features of the Streamlit App:
- Input fields for all required features.
- Real-time predictions using the trained Random Forest model.
- Clear and interactive UI.

---

## Libraries Used

The following libraries were used in this project:

- **NumPy**: For numerical computations.
- **Pandas**: For data manipulation and preprocessing.
- **Matplotlib**: For data visualization.
- **Seaborn**: For advanced visualization.
- **Scikit-learn**: For machine learning algorithms and preprocessing.
- **Streamlit**: For creating the web application.
- **Pickle** and **Joblib**: For saving the trained model.

---

## Steps to Run the Project

### 1. Clone this repository:
```
git clone https://github.com/Jay-patel15/Predictive-maintainance-using-ML
cd predictive-maintenance
```

### 2. Run the Streamlit app:
```
Copy code
streamlit run app.py
```

### 3. Open the app:
The app will automatically open in your default web browser. If it doesn't, navigate to the URL displayed in the terminal (usually http://localhost:8501).

### 4. Use the application:
Enter the required feature values (e.g., air temperature, process temperature, rotational speed, etc.) in the input fields.
The app will predict whether the machine will fail or not based on the provided inputs.

