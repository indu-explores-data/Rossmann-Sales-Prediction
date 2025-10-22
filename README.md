# 🛒 Rossmann Sales Prediction — Forecasting Daily Store Revenue

This project focuses on predicting sales for **Rossmann**, one of the largest drugstore chains in Europe. With over 4,000 stores across multiple countries, accurate sales forecasting is crucial for **inventory planning, promotions, and resource allocation**.  
Through data exploration, feature engineering, and machine learning modeling, this project aims to build a robust sales prediction model using historical store data.

---

## 🧪 Objectives

- Analyze historical **sales and customer trends** across stores.
- Engineer meaningful **time-based and promotional features**.
- Handle outliers to improve model performance.
- Build and compare **machine learning models** for accurate forecasting.
- Identify **key drivers of sales** using feature importance.

---

## 📌 Key Methods & Approach

- **Data Cleaning & Preprocessing**
  - Treated missing values and corrected data types.
  - Removed extreme outliers using the **IQR method**.

- **Feature Engineering**
  - Created **Recency** feature (days since last record).
  - Extracted **Day of Week**, **Promo**, and **Holiday indicators**.
  - Encoded categorical features.

- **Exploratory Data Analysis (EDA)**
  - Sales & customer distribution analysis.
  - Promotion and holiday impact assessments.
  - Correlation and feature significance study.

- **Machine Learning Models**
  - **Decision Tree Regressor**
  - **Random Forest Regressor**
  - **AdaBoost Regressor**
  - **Stacking Regressor**

---

## 📷 Visualizations

### 📊 Distribution & Outliers
![Distribution of Sales, Customers and Recency](images/Distribution%20of%20Sales%2C%20Customers%20and%20Recency.png)  
![Box plot for Sales and Customers (Outliers) and Promo effect on Sales](images/Box%20plot%20for%20Sales%20and%20Customers%20%28Outliers%29%20and%20Promo%20effect%20on%20Sales.png)

### ⏳ Time-based Patterns
![Sales by Day of the Week](images/Sales%20by%20Day%20of%20the%20Week.png)  
![Effect of State Holidays on Sales](images/Effect%20of%20State%20Holidays%20on%20Sales.png)

### 🔍 Feature Relationships
![Feature Correlation Heatmap](images/Feature%20Correlation%20Heatmap.png)  
![Feature Importance](images/Feature%20Importance.png)

### 🤖 Model Performance
![Decision Tree Actual vs Predicted Sales](images/Decision%20Tree%20Actual%20vs%20Predicted%20Sales.png)  
![Random Forest Actual vs Predicted Sales](images/Random%20Forest%20Actual%20vs%20Predicted%20Sales.png)  
![AdaBoost Actual vs Predicted Sales](images/AdaBoost%20Actual%20vs%20Predicted%20Sales.png)  
![Stacking Regressor Actual vs Predicted Sales](images/Stacking%20Regressor%20Actual%20vs%20Predicted%20Sales.png)

---

## 🔍 Key Insights & Outcomes

- **Sales Distribution**
  - Daily sales mostly range from **₹2,000 to ₹10,000**.
  - High-value outliers (>₹15,000) can skew model predictions.

- **Customer Behavior**
  - Most stores serve **<1,000 customers per day**.
  - Sudden spikes (>1,500) act as noise and were treated as outliers.

- **Promotion Impact**
  - **Promo = 1** days show a clear **increase in median sales**.
  - Promotional campaigns are strong revenue boosters.

- **Day of the Week Trends**
  - Sales **drop significantly on Sundays** due to partial/complete store closures.
  - **Weekdays show more stable and higher sales**.

- **Holiday Effects**
  - **State Holidays result in zero or near-zero sales**, indicating closed stores.
  - These dates are essential for forecasting accuracy.

- **Feature Importance**
  - **Customers** is the top predictor of sales.
  - **Promo** and **DayOfWeek** also strongly influence revenue.
  - **Recency** has a minor negative correlation.

- **Model Performance**
  - **Random Forest** and **Stacking Regressor** performed best.
  - Achieved **~85%–86% R² accuracy** on test data.

---

## 💻 Technologies Used

- Python  
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  
- Jupyter Notebook  

---

## 🛠 Setup & Installation

1. Clone the Repository:  
   ```
   git clone https://github.com/your-username/Rossmann-Sales-Prediction.git

   ```
2. Navigate to the Project Directory:
   ```
   cd Rossmann-Sales-Prediction
   ```
3. Create and Activate a Virtual Environment (Recommended):
   ```
   python -m venv venv
   ```
   Windows:
   ```
   venv\Scripts\activate
   ```
   Mac/Linux:
   ```
   source venv/bin/activate
   ```
4. Install Required Libraries:
   ```
   pip install -r requirements.txt
   ```
5. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```
6. Open **Rossmann Sales Prediction.ipynb** and run all cells to reproduce the analysis.

---
## ▶️ **Usage / How to Run**

- Open **Rossmann_Sales_Prediction.ipynb** in Jupyter Notebook
- Run all cells sequentially
- Explore visualizations and model comparisons
- Final forecasts available in model output cells

---

## 🔗 Connect with Me

Let’s connect on LinkedIn for project discussions or data-driven collaborations:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?logo=linkedin)](https://www.linkedin.com/in/indu-r-3a3767170/)

---

## 🙌 Feedback & Support

If you found this project helpful, please ⭐ star the repository and share your thoughts. Suggestions and contributions are always welcome!
   
