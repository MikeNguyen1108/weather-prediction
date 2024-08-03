# Perth Weather Data Analysis
## Project Overview
This project involves scraping, processing, and analyzing 12 years of weather data for Perth from wunderground.com. The goal is to understand historical weather patterns and predict future temperatures using various machine learning models and time series analysis techniques

### Data Collection
We used Selenium to scrape daily weather data from wunderground.com. The data includes various weather parameters such as temperature, dew point, humidity, wind speed, wind gust, and pressure.

### Data Processing
The scraped data was processed to:

+ Combine Date and Time into a single DateTime column.
+ Convert string data to numerical values.
+ Correct Humidity and Pressure values.
+ Remove rows with missing or zero values.
+ Standardize the features using StandardScaler.

### Exploratory Data Analysis
Descriptive statistics and correlation analysis were performed to understand the relationships between different weather variables and identify key predictors for temperature

### Modeling and Prediction
I implemented several machine learning models to predict temperature:

+ Random Forest: Achieved the best performance with high accuracy and low mean squared error.
  
+ K-Nearest Neighbors (KNN): Provided valuable insights but had lower accuracy compared to Random Forest.
  
+ XGBoost: Used hyperparameter tuning with GridSearchCV to optimize the model

### Results

The Random Forest model demonstrated outstanding performance with near-perfect accuracy, minimal prediction errors, and no overfitting. Time series analysis showed clear seasonal patterns in temperature, enabling accurate future predictions.

### Future Work

+ Enhanced Feature Engineering: Incorporate additional weather-related features like precipitation and cloud coverage.
  
+ Advanced Visualization: Develop more detailed visualizations to uncover seasonal patterns and trends.
  
+ Model Deployment: Deploy the model as a web application or API for real-time temperature prediction.
