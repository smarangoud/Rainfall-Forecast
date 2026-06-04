# Rainfall-Forecast
Predicts next 12 months of rainfall using time series analysis (Prophet), capturing seasonal trends and peak rainfall patterns.

##  Project Overview

Rainfall prediction is essential for agriculture, water resource management, and disaster prevention. This project focuses on forecasting rainfall for the next 12 months using historical time series data.

The model also identifies the **maximum rainfall recorded in a single day within a month**, providing deeper insights into rainfall patterns.

---

##  Objectives

*  Forecast rainfall for the next 12 months
*  Identify the highest rainfall in a single day
*  Analyze seasonal rainfall patterns
*  Improve prediction using additional features

---

##  Dataset Description

The dataset consists of multiple CSV files:

* `rainfall-monthly-total.csv` → Monthly total rainfall
* `rainfall-monthly-highest-daily-total.csv` → Max rainfall in a day
* `rainfall-monthly-number-of-rain-days.csv` → Number of rainy days

 Additionally, `.txt` metadata files were used to:

* Understand dataset structure
* Identify missing values (e.g., -999)
* Verify measurement units (mm)

---

##  Data Preprocessing

* Converted date columns into datetime format
* Handled missing values using metadata information
* Merged multiple datasets into a unified dataframe
* Sorted data chronologically

---

##  Exploratory Data Analysis (EDA)

* Visualized rainfall trends using line plots
* Observed strong seasonality patterns
* Identified variations across months

---

##  Feature Engineering

An additional feature was introduced:

* `rain_days` → Number of rainy days per month

This improved model accuracy by capturing rainfall distribution patterns.

---

##  Model Used

This project uses **Facebook Prophet**, a powerful time series forecasting model.

### Why Prophet?

* Handles seasonality automatically
* Works well with missing data
* Easy to interpret
* Suitable for real-world forecasting problems

---

##  Methodology

1. Data collection and preprocessing
2. Feature engineering
3. Train-test split (time-based)
4. Model training using Prophet
5. Model evaluation
6. Forecasting future values
7. Comparison with ARIMA

---

##  Model Evaluation

The model was evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* Cross-validation

---

##  Results

* Successfully forecasted rainfall for 12 months
* Captured seasonal trends effectively
* Improved accuracy using `rain_days` feature
* Identified peak rainfall events

---

##  Model Comparison

| Model   | Strength                 |
| ------- | ------------------------ |
| Prophet | Handles seasonality well |
| ARIMA   | Requires manual tuning   |

Prophet performed better due to its ability to model seasonal patterns.

---

## 📊 Sample Output

* Forecast graph of rainfall trends
* Seasonal decomposition plots
* Maximum rainfall detection

---

##  How to Run the Project

###  Clone Repository

```bash
git clone https://github.com/your-username/Rainfall-Forecasting-Project.git
cd Rainfall-Forecasting-Project
```

###  Install Dependencies

```bash
pip install -r requirements.txt
```

###  Run Notebook

```bash
jupyter notebook
```



---

##  Project Structure

```
Rainfall_Forecasting_Project/
│
├── data/
├── notebook.ipynb
└── README.md
```

---

##  Future Improvements

* Use LSTM (Deep Learning) for better accuracy
* Add temperature and humidity features
* Deploy using cloud platforms
* Real-time rainfall prediction

---

## Key Learnings

* Time series forecasting concepts
* Handling real-world datasets
* Feature engineering for time series
* Model evaluation and comparison

---

##  Contact

If you have any questions or suggestions, feel free to connect!

---

⭐ If you found this project useful, please give it a star!
