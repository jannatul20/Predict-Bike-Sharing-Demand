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


**Discussion**
1. After completing our exploratory analysis we were able to identify trends within the dataset. Rental volume peaked in the month of June, which it was lowest in January. Warmer weather seemed to be an indicator of rental demand. This was supported by temperature being a significant predictor for rental demand, checked via multiple linear regression. This trend isn’t surprising as warmer weather tends to attract people to outdoor activities. Peak rental times throughout weekdays seemed to coincide with what is typically associated with rush hour times, 7:00am-8:00am and 5:00pm-6:00pm. 
2. When looking at weather conditions, more favorable outdoor weather increased rental count. When checked for being a significant predictor, weather was shown not to be a significant predictor. It would be interesting in future work to check multifarious elements of weather conditions, for example higher daily temperatures and unfavorable weather conditions. Also a more detailed dataset may allow a more detailed time series for bike rentals which may show rental demand before, during and after unfavorable weather conditions to check if this changes significance or if it is solely tied to temperature.
3. When checking if Holidays were a significant predictor for rental demand, it was shown through the exploratory analysis and multiple linear regression to be significant. Work days were also a significant predictor, typically you’d expect to see a higher peak demand on a workday then on a weekend or holiday. Weekends saw demand remain relatively steady throughout the day from around 9:00am to 7:00 pm. Seasonal changes in bike rental demand were seen with spring having the lowest demand and fall having the highest. When looking at traits which were seen to be negatively correlated with demand, humidity was deemed to be negatively correlated with rental count. This could be related to the trend we saw with unfavorable weather conditions like precipitation causing an increase in humidity level, more in depth analysis would need to be done with a more detailed dataset, ideally a time series dataset overlaid with weather throughout each day.
4. When assessing models for which worked best, we saw that tree based models had the best result for predicting rental demand. The two best models we assessed were Random Forest and XGBoost. Random forest had a RMSE of 40.093 and RMSLE of 0.309, while XGBoost had an RMSE of 43.248 and RMSLE of 0.302, overall XGBoost was the best model for predicting rental demand as it was the best preforming RMSLE value.


**Conclusion**
Through exploratory analysis and multiple linear regression, we determined following
1. Holidays, working days and temperature to be the only significant predictors for the dataset.
2. Weekdays around rush hour were the highest average peak rental times at 7:00-am - 8:00am and 5:00pm- 6:00pm.
3. Weekends saw steady demand in rentals from 10:00am -6:00pm.
4. Lowest rental counts throughout the year were in spring, while the highest were fall.
5. Finally when looking at the best performing model from our methodology we determined that XGBoost was the best performing model for prediction of rental demand.
6. Other tree based such as Random Forest and Bagging also worked well in prediction of rental demand.


**References**
1. Bike Sharing Demand dataset. Retrieved from Kaggle at this link https://www.kaggle.com/c/bike-sharing-demand on 18th March 2023.​
2. UCI machine learning repository Bike Sharing Dataset. Retrieved from http://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset on 18th March 2023.
