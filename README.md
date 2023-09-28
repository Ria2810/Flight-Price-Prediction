# Flight Price Prediction

This GitHub repository hosts a project for predicting flight fares using machine learning. The project focuses on solving the problem of estimating flight ticket prices based on various features. It includes data description, exploratory data analysis (EDA), feature engineering, model training, and the deployment of a web application for predicting flight prices.

## Table of Contents
1. Introduction
2. Data
3. Exploratory Data Analysis
4. Feature Engineering
5. Feature Selection
6. Model Training
7. Deployment
8. Usage
9. Contributing

## <ins>Introduction </ins>
The main objective of this project is to predict flight ticket prices using machine learning techniques. Accurate flight price prediction is valuable for both travelers and airlines. This project aims to provide users with an estimate of the fare based on various parameters.

## <ins> Data</ins>
The dataset comprises two sets:

- Train Data: 10683 rows and 11 columns.
- Test Data: 2671 rows and 10 columns.
Columns in the dataset include:

- Airline: The airline name.
- - Date_of_Journey: The date of the flight journey.
- Source: The departure location.
- Destination: The arrival location.
- Route: The flight route.
- Dep_Time: The departure time.
- Arrival_Time: The arrival time.
- Duration: The duration of the flight.
- Total_Stops: The number of stops during the flight.
- Additional_Info: Additional information about the flight.
- Price: The target variable, representing the flight fare.
## <ins>Exploratory Data Analysis (EDA)</ins>
EDA was conducted on the dataset, involving:

- Converting Date_of_Journey, Dep_Time, and Arrival_Time into timestamp format for proper use in prediction.
- Handling categorical data using appropriate encoding methods such as OneHotEncoder for nominal data and LabelEncoder for ordinal data.
## <ins>Feature Engineering</ins>
Feature engineering includes preprocessing the test data in the same manner as the training data. This ensures that the data is properly prepared for model training and prediction.

## <ins>Feature Selection</ins>
Feature selection methods were employed using two approaches:

- Heatmap: Correlation analysis to identify important features.
- Feature Importance: Determining the significance of each feature in predicting flight prices.
## <ins>Model Training</ins>
Model training involved the following steps:

- Data splitting into training and testing sets.
- Hyperparameter tuning using RandomizedSearchCV.
- Fitting the data into a Random Forest Regressor.
- Evaluating the model using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared.
- Saving the trained model into a pickle file for future use.
## <ins>Deployment</ins>
A web application was developed using Flask to deploy the trained model. Users can select various input parameters, such as airline, date, source, destination, and more, and click a button to obtain the predicted flight price.

## <ins>Usage</ins>
To use the Flight Price Prediction application:

- Clone this repository to your local machine.
- Install the required dependencies using pip install -r requirements.txt.
- Run the Flask application: python app.py.
- Access the application through your web browser.
## <ins>Contributing </ins>
Contributions to this project are welcome. If you have ideas for improvements or new features, please submit a pull request.
