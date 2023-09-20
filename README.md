# Predict-Bike-Sharing-Demand

This was a group project. Group Members are:
Jannatul Naeema,
Devanshi Patel​​,
Deyvis Dalman,
Faraz Khan​,
Utsav Agrawal.

**Introduction**
Bike sharing programs provide an affordable shared transportation service where bicycles are available for use by individuals for short-distance trips in urban areas, as an alternative to private vehicles. These programs operate similarly to public transit systems, with multiple bike check-out stations catering to both tourists and locals. The aim is to reduce traffic, noise, and air pollution in cities. Bike-share systems offer a sustainable solution for individuals who may have concerns about theft, vandalism, parking, storage, or maintenance of their own bicycles. There are currently over 500 bike-sharing programs worldwide, consisting of more than 500,000 bicycles. These systems generate large amounts of data, making them attractive for research in traffic, environmental, and health issues. The duration of travel, departure and arrival positions are explicitly recorded in these systems, creating a virtual sensor network that can be used to sense mobility in cities. This feature transforms bike sharing systems into virtual sensor networks that can be used to monitor mobility in the city.


**Dataset**
The original dataset is hosted at UCI machine learning repository, contains both daily and hourly count of rental bike data.​The dataset for this project was collected from Kaggle, it is featured in a competition for predict use of a city bikeshare system.​ The dataset was provided by the Capital Bikeshare program in Washington D.C​. This contains the hourly count of rental bikes between years 2011 and 2012 with the corresponding weather and seasonal information. ​It features ~17,000 entries and 12 columns: datetime, season, holiday, working day, weather, temp, avg temp, humidity, windspeed, casual, registered, count​. Training data features the first 19 days of each month, while the test data has the remaining days. Test data does not have the count column, has 9 columns.


**Guiding Questions**
1. Does weather conditions act as significant predictors for bicycle demand within a city?​
2. How does the time of the day impacts bike rental demand?
3. Identify any weekly variation (weekdays, weekends, holidays) and check if any of these are significant predictors.
4. Are there fluctuations in demand based on season?
5. Which techniques are the best for predicting bike rental demand throughout the year?


**Methodology**
We implemented the following techniques on the dataset to test which is best at predicting bike ride share demand:​
Linear regression​, Lasso​, RidgeCV​, Random Forest​, Bagging​, Gradient Boosting​, AdaBoost​, SVR​, KNN​, XGBoost.
