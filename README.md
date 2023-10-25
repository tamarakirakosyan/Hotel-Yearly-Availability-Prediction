# Hotel-Yearly-Availability-Prediction
The purpose of the project is to predict whether the hotel is available 365 days a year or not.

# Data

Column | Description
:---|:---
`id` | The unique ID assigned to every hotel.
`region` | The region in which the hotel is located..
`latitude` | The latitude of the hotel.
`longitude` | The longitude of the hotel.
`accommodation_type` | The type of accommodation offered by the hotel. For example: Private room, Entire house/apt, etc.
`cost` | The cost of booking the hotel for one night. (in \$\$)
`minimum_nights` | The minimum number of nights stay required.
`number_of_reviews` | The number of reviews accumulated by the hotel.
`reviews_per_month` | The average number of reviews received by the hotel per month.
`owner_id` | The unique ID assigned to every owner. An owner can own multiple hotels.
`owned_hotels` | The number of hotels owned by the owner.
`yearly_availability` | It indicates if the hotel accepts bookings around the year. Values are 0 (not available for 365 days in a year) and 1 (available for 365 days in a year).

# Steps and results

- Exploring the data
- Dealing with N/A values
- Converting categorical columns to 0, 1 valued columns to use them in the training
- Feature selection with ANOVA statistical test and correlations
- Spliting the dataset to train and test
- Normalizing the features
- Training the data with Logistic Regression, KNN, Random Forest, XGBoost, CATBoost and LightGBM
- Selecting the best performing model.
- Performing Randomized Search to find the best hyperparameters
- Training the model with the best hyperparameters
- Predicting yearly_availability for test.csv data and extracting the results to submissions.csv file.

As a result we choose XGBoost model and get 93% accuracy predicting yearly availability.

