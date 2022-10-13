## APP Rating Prediction using Machine Learning technique Linea Regression Model building in Python(Pandas,Numpy, Matplotlib,
# Objective
Developed a Machine Learning model to predict the Google apps which have high ratings.

# Problem Statements
Google Play Store team is about to launch a new feature wherein, certain apps that are promising, are boosted in visibility. The boost will manifest in multiple ways including higher priority in recommendations sections (“Similar apps”, “You might also like”, “New and updated games”). These will also get a boost in search results visibility. This feature will help bring more attention to newer apps that have the potential.

# Analysis
Identified  the apps those are promising and boosted visibility. High App ratings,  provided by the customers, have been a  great indicator for predicting the apps ratings.

# Steps Involved
1. load the data
2. check the null values
3. drop the null values
4. formatting the datatypes for the correct model  building
5. Sanity Check
Average rating should be between 1 and 5 as only these values are allowed on the play store. Dropped the rows that have a value outside this range.
Reviews should not be more than installs as only those who installed can review the app. If there are any such records, drop them.
For free apps (type = “Free”), the price should not be >0. Drop any such rows.


