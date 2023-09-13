# Data Science Training from Sprints - Airbnb Challenge

## Team 15 - Predicting Next Custom Travel Trip

**Team Members:**
- Mohamed Aly Elsayed Matar
- Mohamed Abdelmoniem
- Mohamed Fathy
- Karim Ashraf
- Ziad Assem

**Objective:**
We are attempting to predict the next custom travel trip's destination country.

### Data Selection

We have access to six data lists provided by the Airbnb challenge:

1. sample_submisions_NDF
2. countries
3. sessions
4. age_gender_bucket
5. test_users
6. train_users_2

We decided to focus on the following data lists:

- test_users
- train_users_2

We excluded the following data lists for the reasons mentioned:

- sample_submissions_NDF: Not helpful since all destinations are NDF (No Destination Found).
- countries: Contains information about countries, not useful for prediction.
- sessions: Contains user website activity, which may not be relevant for our prediction.
- age_gender_bucket: Contains age and gender information, which is already in the user's data lists.

### Libraries Used

We imported the following libraries for our data analysis and modeling:

- `numpy`: For arrays and matrices.
- `pandas`: For data manipulation and analysis.
- `seaborn`: For data visualization (heat maps, time series, violin plots).
- `matplotlib`: For creating plots and graphs.
- `datetime`: For handling date and time data.
- `itertools`: For iterating over parameter combinations.
- `sklearn`: For modeling and evaluation.
- `statsmodels`: For time series analysis.

### Data Cleaning

We performed data cleaning to prepare the data for analysis and modeling:

- Replaced empty and '-unknown-' values with NaN.
- Set ages outside the range of 15 to 95 to NaN.
- Dropped unnecessary columns.
- Removed rows with NaN values.
- Removed duplicate rows.

### Data Visualization

We visualized various aspects of the data, including:

- Percentage of NULL values in the data.
- Users count by gender.
- Age distribution of users.
- Users count by affiliate channel.
- Users count by affiliate provider.
- Users count by first affiliate tracked type.
- Users' signup method percentage.
- Users' signup app percentage.
- Users count by first device type.
- Users count by first browser.
- Travelers' percentage by country destination.
- Ages' variation with countries (boxplot).

### Time Series Analysis

We analyzed time series data related to user accounts and bookings:

- Converted timestamps to datetime format.
- Plotted time series data for new user accounts created and date of first booking.
- Decomposed the time series data to observe trends, seasonality, and residuals.

### ARIMA Forecasting

We attempted to forecast time series data using the ARIMA model:

- Identified optimal parameters for the SARIMA model.
- Fitted the SARIMA model to the data.
- Plotted model diagnostics.

### Modeling and Prediction

We attempted linear regression to predict the country destination:

- Prepared the data by encoding categorical features.
- Fitted a linear regression model.
- Evaluated the model using R-squared and mean squared error (MSE).

### Random Forest Classifier

We switched to a random forest classifier for prediction:

- Prepared the data by encoding categorical features and scaling.
- Fitted a random forest classifier.
- Calculated model accuracy.

### Challenges

We encountered several challenges during this project:

- Handling non-numerical data.
- The complexity of the project, especially for newcomers to data science.
- The time required to understand and process the data.
- Unexpected issues when using pipelines for training and prediction.

### Conclusion

In this data science project, we explored and visualized Airbnb data to predict the next custom travel trip's destination country. While we faced challenges along the way, we gained valuable experience in data analysis, visualization, and modeling. Our journey in data science continues, and we look forward to tackling more complex projects in the future.
