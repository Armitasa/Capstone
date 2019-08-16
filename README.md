This dataset includes information for users such as age, sex, marital status and education levels, as well as payments and balances for the previous 6 month and wether or not they defaulted on their credit card payment,
The end goal is to train a model that can predict if a customer will default on their payment using the available features.
I started by cleaning the dataset and then creating more relevant features such as the carrying balance and the debt to credit ratio and dropping columns that were not needed.
The next stage was exploratory data analysis to to understand the distribution and to find correlations between the features.
in order to find the best model to predict the defaults I experimented with 3, starting with logistic regression using grid-search for cross-validation. Regression could correctly predict about 77% of the time.
The second model to train was XGboost with an accuracy of 82%. I also used XGboost to find feature importance.
the last model to try was RandomForestClassifier that resulted in test accuracy of 81%.

XGboost appeared to be best model to train the dataset 
