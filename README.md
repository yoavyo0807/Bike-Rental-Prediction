This project contains Python code to solve a regression challenge from the Bar-Ilan Data Science course, predicting the number of bikes rented using various machine learning algorithms.

Goal:

Predict the number of bikes using various regression algorithms.

Challenge Dates:

February 14th, 2024 - February 29th, 2024 (Open only for Bar-Ilan Data Science Students)
Algorithms Used:

Linear Regression
Decision Trees
Random Forest
AdaBoost
XGBoost
Evaluation Metric:

Root Mean Squared Logarithmic Error (RMSLE) is used to evaluate the model performance. This metric is robust to outliers, making it a suitable choice for this competition.

Data:

The data used in this challenge is a real-world dataset from a bike-sharing system. It contains information about factors that might influence bike rentals, such as weather, seasonality, and user type.

Data Description:

Source: Bike-sharing system (source not explicitly provided)
Type: Real-world
File format: CSV (Comma-separated values)
Files:
train.csv: Training data set
test.csv: Testing data set (without target variable)
sampleSubmission.csv: Sample submission file in the correct format
Data Fields:
datetime: Hourly date and timestamp
season: Season (1 = spring, 2 = summer, 3 = fall, 4 = winter)
holiday: Whether the day is considered a holiday (binary)
workingday: Whether the day is neither a weekend nor holiday (binary)
weather: Weather condition code (categorical)
temp: Temperature in Celsius
atemp: "Feels like" temperature in Celsius
humidity: Relative humidity
windspeed: Wind speed
casual: Number of non-registered user rentals initiated
registered: Number of registered user rentals initiated
count: Number of total rentals (target variable to be predicted)
Usage:

Clone this repository.
Install dependencies. You will need libraries like scikit-learn and XGBoost. Refer to their documentation for installation instructions.
Place your data in a folder named data within the project directory. Ensure the data matches the format described above.
Run the script. The script (main.py) is not provided here, but it should iterate through the defined models, train them on the data, make predictions, and calculate the RMSLE for each model.
Evaluation:

The RMSLE score for each model will be printed to the console. You can compare these scores to assess the performance of each model on this dataset.
