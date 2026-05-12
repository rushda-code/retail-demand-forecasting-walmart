# Retail Demand Forecasting — Walmart Dataset

-----

## Overview
This project builds an end-to-end retail demand forecasting system using Walmart sales data.  
It explores sales trends, performs feature engineering, and applies multiple models to predict weekly sales.

## Objective
- Analyze historical sales patterns
- Understand the impact of holidays and external factors
- Build forecasting models
- Compare model performance
- Generate business insights

---

## Dataset
Source: Walmart Weekly Sales Dataset (Kaggle)

Files used:
- train.csv
- features.csv
- stores.csv

### Key Features
- Store, Dept, Date
- Weekly_Sales (target)
- Temperature, Fuel_Price
- CPI, Unemployment
- MarkDown1–5
- Store Type, Size
- IsHoliday

---
## Project Structure


├── Retail_Demand_Forecasting_Walmart.ipynb

├── README.md

├── requirements.txt

└── data/

└── README.md


---

## Workflow

### 1. Data Preparation
- Merged train, features, and store datasets
- Handled missing values
- Converted categorical variables

### 2. Exploratory Data Analysis
- Sales trends over time
- Store type comparison
- Holiday impact analysis
- Correlation heatmap
- Seasonal decomposition

### 3. Feature Engineering
- Date features (Year, Month, Week, etc.)
- Lag features (1, 4, 12 weeks)
- Rolling averages (4-week, 12-week)

### 4. Models Used

#### Prophet
- Time series forecasting model
- Used for single store and department
- Captures trend and seasonality

#### XGBoost
- Gradient boosting model
- Trained on full dataset
- Best performance in RMSE

#### LSTM
- Deep learning model for sequential data
- Applied on single time series
- Captures temporal dependencies

---

## Evaluation Metrics
- RMSE (Root Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)

---

## Results Summary
| Model     | Performance |
|----------|------------|
| XGBoost  | Best RMSE |
| Prophet  | Best MAPE |
| LSTM     | Moderate performance |

---

## Key Insights
- Sales show strong seasonality
- Holidays significantly impact demand
- Larger stores generate higher sales
- Lag features are highly predictive

---

## Business Applications
- Inventory optimization
- Workforce planning
- Promotion timing
- Demand planning

---

## Limitations
- Limited data for deep learning models
- No SKU-level granularity
- External events not included

---

## Future Improvements
- Ensemble models (Prophet + XGBoost)
- Add external data (weather, events)
- Store-level or department-level models
- Hyperparameter tuning

---

## Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- XGBoost
- Prophet
- TensorFlow / Keras
- Scikit-learn

---

## Author
RUHDA ASLAMI

*[https://github.com/rushda-code]*

*[https://www.linkedin.com/in/rushda-aslami]*


---

