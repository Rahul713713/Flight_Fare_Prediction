# Flight Fare Prediction : Project Overview
![Flight_Fare_Prediction](https://github.com/Rahul713713/Flight_Fare_Prediction/blob/main/indigo.png "Flight Fare Prediction")
- Created multiple charts,graphs,countplots,etc. in order to understand how price varies with different features.
- Worked on a dataset consisting of 10683 rows of data for 10 different features.
- Performed univariate analysis as well as multivariate analysis on various features to understand the importance of every feature.
- Performed data cleaning, data preprocessing and exploratory data analysis to understand the independent variables and prepare the data for modeling.
- Implemented multiple regression algorithms and came up an r square value of 0.85 with XGB.


# Problem Statement
Predict the ticket prices of flights based on multiple independent variables and machine learning algorithms.

The data that I have contains information such as Airline,Date_of_Journey,Source,Duration,etc. and I have to predict price of the tocket based on these features and machine learning.

# Code and Resources Used
- Packages: pandas, numpy, matplotlib, seaborn, scikit-learn

# Data Cleaning and Preprocessing
## After reading the data, I needed to clean it up so that it would be fit for our data analysis. I made the following changes and created the following variables:
- Checked whether we have missing data for various columns.
- Some columns had missing values. I dropped those rows as there were only 2 rows with missing data.
- Performed Data Standardisation to get the data on the same scale with the mean of 0 and standard deviation of 1.
- Finally,the columns used for EDA are

 1   Airline          
 2   Date_of_Journey  
 3   Source           
 4   Destination      
 5   Route            
 6   Dep_Time         
 7   Arrival_Time     
 8   Duration         
 9   Total_Stops      
 10  Additional_Info  
 11  Price                 

# EDA
After cleaning the data,I started with EDA. These are some of the outcomes of EDA 

![Flight_Fare_Prediction](https://github.com/Rahul713713/Flight_Fare_Prediction/blob/main/Most_Used_Airlines.png "Most_used_airlines")
![Flight_Fare_Prediction](https://github.com/Rahul713713/Flight_Fare_Prediction/blob/main/price_vs_airplanes.png "Price_vs_Airlines")
![Flight_Fare_Prediction](https://github.com/Rahul713713/Flight_Fare_Prediction/blob/main/Feature_Importance.png "most_important_features")

# Machine Learning Models
- The Machine Learning Models that I've used are as follow:

 1   Linear Regression              
 2   Decision Tree              
 3   Random forest             
 4   XGB           

# Result

    +-----------------------------------------------------------------------------------+
    | *** Model Summary *** [Performance Metric: R squared(Coefficient Of Determination)] |
    +--------------------------------+---------------+---------------+------------------+
    |           Model Name           |      MAE      |      RMSE     |    R squared     |
    +--------------------------------+---------------+---------------+------------------+
    |       Linear Regression        |    1927.93    |      2418     |       0.62       |
    |         Decision Tree          |    1328.57    |      2418     |       0.73       |
    |         Random forest          |    1183.04    |    2096.69    |       0.8        |
    |              XGB               |    1135.49    |    1820.25    |       0.85       |
    +--------------------------------+---------------+---------------+------------------+
