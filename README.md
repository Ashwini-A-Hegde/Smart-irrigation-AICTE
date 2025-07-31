# 🌱 Smart Automated Irrigation System using Soil Moisture and Weather Data

This project leverages soil moisture levels, environmental data, and machine learning to create an intelligent irrigation system that conserves water and enhances crop health. Designed for smart agriculture, it controls pump activation based on real-time data and predictive analysis.

## 📌 Features

- Collects and analyzes **soil moisture, humidity, temperature, and weather conditions**
- Trains a **Random Forest Classifier** to predict irrigation need
- Controls water **pump activation** automatically
- Saves water and energy through data-driven irrigation scheduling
- Supports future integration with IoT sensors and cloud platforms

---

## 🧠 Technologies Used

- Python(3.12.4)
- VS Studio Code+Jupyter Notebook Extension
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (RandomForest, MultiOutputClassifier)
- Joblib for model persistence

---

## 📁 Dataset Overview

The dataset includes:
- `soil_moisture`
- `temperature`
- `humidity`
- `weather_condition` (categorical)
- `pump_status` (on/off labels)

Make sure the dataset file `smart_irrigation_dataset.csv` is in the same directory as the ipynb file.

---

## 🚀 How It Works

1. **Data Loading and Preprocessing**
   - Dataset is loaded using `pandas`
   - Unnecessary columns like `Unnamed: 0` are dropped
   - Features are scaled using `MinMaxScaler`

2. **Model Training**
   - A `RandomForestClassifier` is trained to predict the irrigation requirement
   - MultiOutputClassifier is used for multiple target predictions if applicable
   - Evaluation is done using classification report

3. **Model Saving**
   - The trained model is saved using `joblib`
   - Ready to be deployed with sensor data integration for real-time predictions

---

## 🛠️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Ashwini-A-Hegde/smart-irrigation.git
   cd smart-irrigation
