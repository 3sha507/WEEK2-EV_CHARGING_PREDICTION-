# 🔋 Electric Vehicle Charging Demand Forecasting

This project is developed as part of the **AICTE Internship – July 2025**, under IBM Edunet Foundation. It forecasts the **demand for electric vehicle (EV) charging infrastructure** using historical EV registration data and deploys the model as a web application.

---

## 🗂️ Weekly Breakdown

### ✅ Week 1: Data Preprocessing & Exploration
- Loaded raw dataset: `Electric_Vehicle_Population_By_County.csv`
- Cleaned missing values, removed duplicates
- Converted dates and extracted useful time features
- Performed exploratory data analysis (EDA)
- Saved processed data as: `preprocessed_ev_data.csv`

### ✅ Week 2: Model Training & Forecasting
- Selected features like County, Model Year, Vehicle Type
- Applied Random Forest Regressor to forecast EV adoption
- Evaluated model using R² Score and RMSE
- Saved trained model using `joblib` as: `forecasting_ev_model.pkl`
- Visualized EV growth for top counties
- Final notebook: `Week2_EV_Charging_Demand.ipynb`

### ✅ Week 3: Deployment
- Created a Python script `app.py` to deploy model
- Used `Flask` to build a web API for predictions
- Reads user input (e.g., County, Model Year) and returns forecast
- Ensures reusability by loading preprocessed data and saved model
- Deployment-ready structure prepared

---

## 🔍 Project Overview

### 🎯 Goal:
To **forecast future EV adoption trends** so planners and stakeholders can optimize EV charging infrastructure in various U.S. counties.

### 🔧 Tech Stack:
- **Python** (Pandas, Scikit-learn, Flask, Matplotlib)
- **Google Colab** (for notebook execution)
- **GitHub** (version control)
- **Flask** (API deployment)
- **joblib** (model serialization)

---

## 📁 File Structure

```plaintext
EV_Vehicle_Charge_Demand/
├── Electric_Vehicle_Population_By_County.csv   # Raw data
├── preprocessed_ev_data.csv                    # Cleaned & saved dataset
├── forecasting_ev_model.pkl                    # Trained model
├── Week2_EV_Charging_Demand.ipynb              # Full notebook (Week 1 + 2)
├── app.py                                      # Flask app for deployment (Week 3)
├── requirements.txt                            # Python dependencies
├── ev-car-factory.jpg                          # Image asset (optional)
└── README.md                                   # Project documentation
```

---

## 🚀 How to Run Locally

### 1. 🔧 Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. ▶️ Run the Flask App
```bash
python app.py
```

### 3. 🌐 Access in Browser
Open your browser and go to:
```
http://127.0.0.1:5000
```

You’ll be able to input parameters and receive EV demand predictions.

---

## 📊 Model Insights

- **Algorithm:** Random Forest Regressor
- **Input Features:** County, Model Year, Electric Vehicle Type
- **Output:** Forecasted number of EVs in future
- **Evaluation Metrics:** R² Score, MAE, RMSE

---

## 📌 Improvisations Done

- Regenerated and saved clean dataset from raw input
- Feature engineering for improved model performance
- Trained a reusable and tunable model from scratch
- Saved both preprocessed data and trained model
- Built a deployable Flask app using modular, readable code

---

## 💡 Future Scope

- Host app on **IBM Cloud / Render / Streamlit Cloud**
- Add interactive dashboard (e.g., Streamlit or Dash)
- Integrate real-time data streams for live forecasting


