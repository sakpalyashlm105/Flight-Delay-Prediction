# Flight-Delay-Prediction

This project aims to predict if a flight will be delayed by more than 30 minutes before its departure, using available data from airports and airlines.

### 1. Data
The dataset is from Kaggle on airlines delays from the U.S. Department of Transportation's Bureau of Transportation Statistics. It tracks the on-time performance of domestic flights operated by large air carriers.

The features include information on the date, scheduled departure/arrival times, actual departure/arrival times, flight numbers, origin and destination airports etc. The target variable is a binary indicator of whether the actual departure time was delayed by more than 30 minutes from the scheduled departure time.

### 2. Exploratory Data Analysis

* Performed initial data cleaning and preprocessing
* Created new features such as day of week, month from date variables
* Analyzed frequency of delays, top origins/destinations
* Studied airline, aircraft, airport features
* Looked at seasonal trends
* Identified and handled missing values

### 3. Feature Engineering

* Extracted time components from departure/arrival times
* Applied trigonometric transformations for cyclic features
* Binned airlines, airports into categories
* Added airline, aircraft, airport historical averages
* Log transformed skewed features
* Encoded categorical variables

### 4. Modeling

* Compared Logistic Regression, SVM, Decision Tree and Random Forest models
* Tuned hyperparameters using HalvingGridSearch cross-validation
* Evaluated models using precision-recall curves, ROC curves, F1 scores
* Chose best model based on performance and business cost-benefit analysis

### 5. Conclusion

The Random Forest classifier performed the best with F1 score of 0.93 on test data. Feature importances showed flight delay causes and temporal features as most predictive. The model can help airlines better schedule flights and manage resources.
