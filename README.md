# Isolation Forest Anomaly Detection Streamlit App

A Machine Learning project that uses the **Isolation Forest Algorithm** to detect anomalies (outliers) in customer data through an interactive Streamlit web application.

---

## Overview

Isolation Forest is an unsupervised machine learning algorithm used for anomaly detection. It works by isolating observations through random partitioning and identifies unusual data points that differ significantly from the majority of the dataset.

This application allows users to input customer information and determine whether the customer is considered **Normal** or an **Anomaly**.

---

## Features

- Data preprocessing pipeline
- Feature scaling using StandardScaler
- Anomaly detection using Isolation Forest
- Interactive Streamlit interface
- Real-time anomaly prediction
- Clean project architecture
- Easy deployment on Streamlit Cloud

---

## Project Structure

```text
IsolationForest_Streamlit/
│
├── data/
│   ├── raw/
│   │   └── Mall_Customers.csv
│   │
│   └── processed/
│       └── cleaned_data.csv
│
├── models/
│   ├── isolation_forest_model.pkl
│   └── scaler.pkl
│
├── notebooks/
│   └── EDA.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── train_model.py
│   └── predict.py
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Dataset

This project uses the Mall Customers Dataset.

### Features Used

- Age
- Annual Income (k$)
- Spending Score (1-100)

The model learns the normal behavior of customers and identifies unusual patterns.

---

## Technologies Used

- Python
- Streamlit
- Pandas
- NumPy
- Scikit-Learn
- Joblib
- Matplotlib
- Seaborn

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Anusreereddysama/IsolationForest.git
```

Navigate to the project directory:

```bash
cd IsolationForest
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Data Preprocessing

Run:

```bash
python src/data_preprocessing.py
```

This step:

- Loads the dataset
- Removes unnecessary columns
- Selects relevant features
- Saves cleaned data

---

## Model Training

Run:

```bash
python src/train_model.py
```

This step:

- Scales the data
- Trains the Isolation Forest model
- Saves the trained model
- Saves the scaler

---

## Running the Streamlit Application

```bash
streamlit run app.py
```

---

## Machine Learning Workflow

```text
Raw Dataset
      │
      ▼
Data Preprocessing
      │
      ▼
Feature Scaling
      │
      ▼
Isolation Forest Training
      │
      ▼
Anomaly Detection
      │
      ▼
Streamlit Interface
```

---

## Prediction Output

The application classifies customer records as:

### Normal Customer

```text
Prediction: Normal Customer
```

### Anomalous Customer

```text
Prediction: Anomaly Detected
```

---

## Applications of Isolation Forest

- Fraud Detection
- Financial Risk Analysis
- Credit Card Fraud Detection
- Intrusion Detection
- Network Security
- Manufacturing Defect Detection
- Healthcare Monitoring
- Customer Behavior Analysis

---

## Future Enhancements

- Interactive anomaly visualization
- User dataset upload
- Multiple anomaly detection algorithms
- Download prediction reports
- Real-time anomaly monitoring dashboard
- Feature importance analysis

---

## Learning Outcomes

This project helps in understanding:

- Unsupervised Learning
- Anomaly Detection
- Isolation Forest Algorithm
- Feature Scaling
- Model Deployment
- Streamlit Application Development

---

## Requirements

```txt
streamlit
pandas
numpy
scikit-learn
joblib
matplotlib
seaborn
```

---

## Author

**Anusree Reddy**

GitHub:

https://github.com/Anusreereddysama

---

## License

This project is developed for educational and learning purposes.
