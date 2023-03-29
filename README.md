#Bike Sharing Demand Prediction
This project aims to predict the hourly bike rental demand using the Bike Sharing dataset from the UCI Machine Learning Repository.

#Dataset
The dataset contains hourly rental data spanning two years. The training set contains data from the first 19 days of each month, while the test set contains data from the remaining days.

#The dataset contains the following features:

datetime: hourly date + timestamp
season: 1 = spring, 2 = summer, 3 = fall, 4 = winter
holiday: whether the day is considered a holiday
workingday: whether the day is neither a weekend nor a holiday
weather:
1: Clear, Few clouds, Partly cloudy, Partly cloudy
2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
temp: temperature in Celsius
atemp: "feels like" temperature in Celsius
humidity: relative humidity
windspeed: wind speed

#The target variable is:
count: number of total rentals

#Methodology
#Data exploration and visualization to understand the relationships between different features and the target variable.
#Feature engineering: create new features such as year, month, hour, weekday, day of the month, and rush hour.
#Data preprocessing: split the dataset into training and test sets.
#Model selection: use the Random Forest Regressor for prediction.
#Hyperparameter tuning: perform an exhaustive search over the specified parameter grid using GridSearchCV to find the best parameters for the Random Forest Regressor model.
#Model evaluation: measure the performance of the model using the Root Mean Squared Log Error (RMSLE) metric.

#Dependencies
Python 3.8+
pandas
numpy
matplotlib
seaborn
scikit-learn

#Usage
Cloned this repository.
Installed the required dependencies.
Ran the Jupyter Notebook or Python script containing the data analysis and prediction steps.

#The Results
The Random Forest Regressor model with the best hyperparameters found by GridSearchCV was used to predict the bike rental demand on the test dataset. The model's performance was evaluated using the RMSLE metric. Further improvements can be made by exploring different machine learning algorithms or by engineering additional features.




