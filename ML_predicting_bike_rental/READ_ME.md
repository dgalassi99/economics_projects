**Machine Learning Project: Pedal Predictors Team**

**Objective:**
The primary goal of this project was to **accurately forecast the number of hourly bicycle rentals** for Mule, a new short-term bike rental company in Geneva, over the next three months. This forecast is essential for securing bank loans and ensuring operational success.

**Data:**
The project used **temporal and meteorological data** from a similar company in another country, structured as an hourly time series.
*   The **training dataset** contained 15211 hourly observations over 21 months.
*   The **test dataset** covered the last three months of 2012 (2168 observations) and contained the same predictors but lacked the target variable (`cnt`).
*   Predictors included date, season, year, month, hour, holiday status, weekday, working day status, weather situation, normalized temperature, feeling temperature, humidity, and wind speed.

**Methodology:**
Our approach involved several key steps:
1.  **Data Preprocessing:** Handled missing values using specific filling techniques based on variable type and removed the remaining 0.289%.
2.  **Exploratory Data Analysis (EDA):** Analyzed the data to understand patterns, including the time series nature, seasonality, hourly usage peaks (different for working vs. non-working days), and the influence of weather (temperature, windspeed).
3.  **Feature Engineering:** Created new features and transformed existing ones to improve model performance. This included encoding categorical variables, generating interaction terms (e.g., weather, time), incorporating cyclical patterns using sinusoidal functions for hour and month, classifying time-of-day intervals, creating `hour_pick` for peak time differences, adding binary spike/drop flags, and introducing lagging features and rolling statistics. Outlier detection using z-scores was also explored. Correlation analysis helped identify relevant and redundant features.
4.  **Train/Test Split and Cross Validation:** Used a **non-shuffled 70/30 split** and **TimeSeriesSplit** for cross-validation to maintain the chronological order of the data.
5.  **Modeling:** Evaluated various machine learning models, including Linear Regression, KNN, Ridge, Lasso, Gradient Boosting, Decision Trees, Bagging, Random Forest, and Recurrent Neural Networks (RNNs), primarily using **Mean Absolute Error (MAE)**.

**Results and Final Model:**
While models like Bagging and Random Forest showed strong performance with low OOB/train errors, these results did not consistently translate to the best performance on external evaluation. Therefore, **Gradient Boosting was selected as the final model** for predicting rentals on unseen data, as it provided the best results in that context.

**Business Insights:**
The analysis provides key insights for Mule:
*   An **increasing trend** suggests potential for expansion.
*   **Seasonality and weather patterns** require strategic planning for fleet availability, maintenance, and promotions.
*   **Time-of-day differences** between working days and weekends allow for tailored initiatives like specific pricing or partnerships.
*   Future data collection could include metrics like bike availability, location-based demand proxies, and traditional transportation costs to enhance insights and predictions.

**Conclusion:**
This project successfully delivered forecasting tools and actionable insights using machine learning, providing Mule with the means to optimize operations, ensure financial stability, and contribute effectively to Geneva's urban mobility.
