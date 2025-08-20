# 🛒 Rossmann Sales Prediction Project  

This project focuses on predicting sales for Rossmann, one of the largest drugstore chains in Europe. With over 4,000 stores across multiple countries, Rossmann generates billions in revenue each year. Accurate sales forecasting is critical for effective inventory management, promotional planning, and resource allocation.  

The goal of this project is to analyze sales data, perform feature engineering, handle outliers, and build machine learning models to forecast daily sales.  

---

## 📌 Key Steps  

1. **Data Exploration & Cleaning**  
   - Handled missing values and ensured correct data types (e.g., treating `StateHoliday` as categorical).  
   - Removed outliers using the **IQR method** for features like `Customers`.  

2. **Feature Engineering**  
   - Created **Recency** feature (days since last sale record).  
   - Extracted useful time-based features like **day of week**.  
   - Encoded categorical variables for modeling.  

3. **Exploratory Data Analysis (EDA)**  
   - Distribution of Sales, Customers, and Recency  
   - Outlier analysis with box plots  
   - Effect of promotions and state holidays on sales  
   - Correlation heatmap for features  

4. **Modeling**  
   Implemented and compared multiple models:  
   - Decision Tree Regressor  
   - Random Forest Regressor  
   - AdaBoost Regressor  
   - Stacking Regressor  

   Feature importance was extracted to understand key drivers of sales.  

---

## 📊 Visualizations  

### Distribution & Outliers  
![Distribution of Sales, Customers and Recency](images/Distribution%20of%20Sales%2C%20Customers%20and%20Recency.png)  
![Box plot for Sales and Customers (Outliers) and Promo effect on Sales](images/Box%20plot%20for%20Sales%20and%20Customers%20%28Outliers%29%20and%20Promo%20effect%20on%20Sales.png)  

### Time-based Patterns  
![Sales by Day of the Week](images/Sales%20by%20Day%20of%20the%20Week.png)  
![Effect of State Holidays on Sales](images/Effect%20of%20State%20Holidays%20on%20Sales.png)  

### Feature Relationships  
![Feature Correlation Heatmap](images/Feature%20Correlation%20Heatmap.png)  
![Feature Importance](images/Feature%20Importance.png)  

### Model Performance  
![Decision Tree Actual vs Predicted Sales](images/Decision%20Tree%20Actual%20vs%20Predicted%20Sales.png)  
![Random Forest Actual vs Predicted Sales](images/Random%20Forest%20Actual%20vs%20Predicted%20Sales.png)  
![AdaBoost Actual vs Predicted Sales](images/AdaBoost%20Actual%20vs%20Predicted%20Sales.png)  
![Stacking Regressor Actual vs Predicted Sales](images/Stacking%20Regressor%20Actual%20vs%20Predicted%20Sales.png)  

---

## 📈 Final Summary of Findings  

- **Sales Distribution**  
  - Most daily sales fall between **₹2,000 and ₹10,000**.  
  - A few records exceed **₹15,000**, which are statistical outliers that can skew averages and reduce model accuracy.  

- **Customer Behavior**  
  - Daily customer counts are typically **below 1,000**.  
  - Occasional spikes above **1,500** act as outliers and may introduce noise into predictions.  

- **Impact of Promotions**  
  - Days with **active promotions (Promo = 1)** show **higher median sales** and greater variability.  
  - Confirms that promotional campaigns significantly boost store revenue.  

- **Day of the Week Patterns**  
  - **Sales dip sharply on Sundays (DayOfWeek = 7)** due to full or partial closures.  
  - Weekdays (Monday–Friday) show **higher and more stable sales** levels.  

- **Effect of Holidays**  
  - Sales are **significantly lower or zero on state holidays**, indicating widespread closures.  
  - These dates are critical to consider in forecasting.  

- **Recency Feature**  
  - The engineered **Recency** variable (days since last recorded date) shows a **slight negative correlation** with sales.  
  - Suggests that **recent data has greater predictive value**.  

- **Feature Importance**  
  - **Customers** is the most impactful predictor.  
  - **Promo** and **DayOfWeek** follow in importance.  
  - **SchoolHoliday** and **Recency** contribute less to model performance.  

- **Model Performance**  
  - **Random Forest** and **Stacking Regressor** achieved the best results.  
  - Both models delivered **R² scores of ~85%–86%**, showing strong predictive accuracy on unseen data.  

---

## 📬 Connect with Me  

If you found this project interesting, let’s connect!  

🔗 [LinkedIn](https://www.linkedin.com/in/indu-r-3a3767170/)  

---

✨ *This repository demonstrates the full pipeline of data preprocessing, exploratory analysis, and machine learning modeling for a real-world retail sales prediction problem.*  
