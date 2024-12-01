***Crash Risk Prediction and Analysis:***

The Transportation Data Science Project (TDSP) leverages open data to create data-driven insights aimed at improving road safety. Through this project, participants use data science techniques such as data cleaning, geospatial analysis, and time-series analysis to assess road conditions, contributing factors, and more. By engaging in real-world datasets, learners are equipped to build analytical models for safer transportation. The project fosters collaboration and learning, offering different tracks for learners based on their experience, with the opportunity to present findings to mentors from the U.S. Department of Transportation.
https://nebigdatahub.org/nsdc/tdsp/

This project aims to predict high-risk crash locations and analyze contributing factors using machine learning techniques. By leveraging historical crash data and various features such as geographic location, crash severity, and contributing factors, the goal is to create a predictive model that can forecast future crashes. We use the XGBoost algorithm to train the model, and visualize the results using interactive maps and heatmaps to highlight high-risk zones. This approach can be used to improve traffic safety by identifying areas that require intervention.

**Dataset**
https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95/about_data

**Project Structure:**
*Data Preprocessing:*
Clean and process the crash data, handling missing values and scaling relevant features.

*Feature Engineering:*
Identify and create new features, including geographical, temporal, and contributing factors, to enhance the model’s predictive power.

*Model Training (XGBoost):*
Train an XGBoost model to predict high-risk crashes based on the available features.

*Heatmap and Map Visualization:*
Visualize the crash data using seaborn heatmaps and interactive folium maps, displaying high-risk crash locations and contributing factors.

**Dependencies**
Python 3.x
pandas
numpy
matplotlib
seaborn
folium
scikit-learn
xgboost

**Features**
*Crash Severity:*
The dataset includes information on the severity of crashes, used as a key feature in predicting high-risk zones.

*Contributing Factors:*
This includes factors like weather, road conditions, and time of day, which are critical for understanding why certain areas are high-risk.

*Geospatial Data:*
The dataset contains latitude and longitude data for each crash, allowing us to visualize crash locations on maps and identify geographical patterns.

*Risk Prediction:*
The XGBoost model predicts high-risk crash zones based on historical data, taking into account severity and contributing factors.

*Visualization*
Heatmap: A heatmap is used to show areas with the highest crash severity by day and hour.
Folium Map: Interactive map visualizes high-risk areas and allows inspection of contributing factors for each crash.

**Results**
The XGBoost model achieved an accuracy of 76.40% in predicting high-risk crash locations.
Heatmaps show patterns in crash severity, with high-risk periods identified from 3 PM to 6 PM and Wednesday to Friday.
The interactive folium map reveals the contributing factors for high-risk crashes, such as poor road conditions, enabling targeted interventions.

<img width="628" alt="Screenshot 2024-12-01 at 1 19 14 PM" src="https://github.com/user-attachments/assets/386b2f9d-2cd7-418a-b7b0-445a91f4fb1d">

Understanding low to high risk level on map 

<img width="641" alt="Screenshot 2024-12-01 at 1 19 27 PM" src="https://github.com/user-attachments/assets/94a157f3-9c58-47da-8387-056d39f404af">

Predicting future possible crashes based on train model

<img width="834" alt="Screenshot 2024-12-01 at 1 19 42 PM" src="https://github.com/user-attachments/assets/520e231d-9c10-4c5c-beb0-4a31f9b7d05c">

understanding contributing factor on future crash to prevent them from happening 


**Future Improvements**
*Incorporate More Features:*
Add additional features like traffic volume or time of day, and integrate real-time data (weather conditions, traffic updates) to improve predictions.

*Model Optimization:*
Improve model accuracy by performing further hyperparameter tuning, handling imbalanced data using techniques like SMOTE, and incorporating cross-validation.

*Advanced Machine Learning Models:*
Explore other models such as LightGBM or Random Forests, or combine them using ensemble methods for improved results.

*Explainability:*
Use tools like SHAP or LIME to interpret the model’s predictions and better understand the factors influencing crash severity.

**Conclusion**
This project provides valuable insights into crash patterns and identifies high-risk locations where interventions can be implemented. By leveraging machine learning techniques and data visualization tools, this approach can help improve traffic safety and reduce the occurrence of severe crashes. Future improvements will continue to enhance the model’s accuracy and predictive power, providing more actionable insights for traffic safety management.


