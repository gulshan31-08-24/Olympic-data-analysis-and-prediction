![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)

# 🏅 Olympic Data Analysis and Prediction

## 📌 Project Overview
This project performs a **comprehensive analysis of 120 years of Olympic Games data** and predicts the **probability of an athlete winning a medal** using **machine learning algorithms** such as **Logistic Regression**.  

The project consists of:
- **Exploratory Data Analysis (EDA):** Understanding trends, participation, and medal distributions over the years.  
- **Prediction Model:** Estimating the medal-winning probability of a particular athlete using past data.  
- **Deployment Ready Scripts:** Streamlit-based `app.py` to run the project with trained models.
- **How to Run:** `streamlit run app.py` write this command in terminal.

---


## 📂 Project Structure
- app.py → Main application file (Streamlit app)
- helper.py → Utility functions for data analysis
- preprocessor.py → Data preprocessing and feature engineering
- modellr.pkl → Saved Machine Learning model (Logistic Regression)
- transformer.pkl → Saved transformer (scaler/encoder for preprocessing)
- athlete_events.csv → Main dataset with Olympic athlete records
- noc_regions.csv → Dataset mapping NOC codes to regions

---
## ⚙️ How to Run the Project

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/olympic-data-analysis.git
   cd olympic-data-analysis
2.**Install Dependencies**

3.**Run the Streamlit App**
  `streamlit run app.py`
    
4.**Open in Browser**
 `http://localhost:8501/`


---
## 📊 Datasets Used

### 1. athlete_events.csv
- Contains detailed records of Olympic athletes from **1896 to 2016**.  
- **Columns include:**  
  - `Name`, `Sex`, `Age`, `Height`, `Weight`  
  - `Team`, `NOC`, `Games`, `Year`, `Season`, `City`  
  - `Sport`, `Event`, `Medal`  

### 2. noc_regions.csv
- Provides mapping of **National Olympic Committee (NOC) codes** to country/region names.  
- **Columns include:**  
  - `NOC` → National Olympic Committee code  
  - `region` → Country/Region name  
  - `notes` → Additional details (if any)
 
---
## 📦 Important Libraries Used
- Pandas → Data manipulation and analysis
- NumPy → Numerical computations
- Matplotlib → Data visualization
- Seaborn → Statistical data visualization
- Scikit-learn → Machine learning algorithms, preprocessing, and model saving
- Flask / Streamlit → Web framework for deployment
- Pickle / Joblib → Model serialization

---
## 📈 Features
- **Medal Tally** → View medal counts by year, country, or overall
- **Medal Predictor** → Predict the probability of an athlete winning a medal
- **Overall Analysis** → Explore trends across 120 years of Olympic data
- **Country-wise Analysis** → Drill down into performance of specific countries
- **Athlete-wise Analysis** → Analyze individual athlete performance and history

---
## 🤖 Machine Learning Model Integration
- **Logistic Regression** is used as the baseline model
- Features considered: Age, Height, Weight, Sex, Sport, etc.
- Data preprocessing performed using transformer (scaling & encoding)
- Trained model saved as `modellr.pkl`
- Preprocessing pipeline saved as `transformer.pkl`

---
## 🚀 Future Improvements
- Experiment with advanced models such as Random Forest, XGBoost, or Neural Networks
- Perform hyperparameter tuning for better accuracy
- Improve feature engineering by incorporating historical athlete performance
- Add visual dashboards for interactive analysis
- Deploy on cloud platforms (Heroku, AWS, Streamlit Cloud) for public access






