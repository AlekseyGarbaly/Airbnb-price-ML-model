# Airbnb-price-ML-model
Exploring Machine learning models that best predict Airbnb prices in Minneapolis

In this project the goal was to use various learned machine learning model and practices to find a model that was able to predict Airbnb prices most accurately. This was a group project and there is a paper that can be provided upon request.

The Data folder contains the Tableau packaged workbooks that incluenced which variables should be used for the model and the resulting csv files that ended up being utiolized bu the models. The varibales that were disregarded weere determined by looking for correlation, skewness, variable dependence, etc.

List of regression models used: Multiple linear regression, polynomial regression, decisioin tree (regression & assification), random forest (regression & classification). 
List of classifidcation models used: Logistical regression, K nearest neighbor (K-NN), Support Vector Machine (SVM), Kernel SVM, Naives Bayes.
In Classiciation Model #1 all rows of the "Review Score Rating" column containing missing values were deleted whereas in Model #2 all missing cells were replaced with zero's.
In Regression model #1, it contained only numerical columns and it deleted the columns; ‘'cancellation policy,' 'bathrooms,' and 'minimum nights'. In Regression Model #2 it contained both numerical and binary categorical columns and it deleted the columns; ‘'cancellation policy,' 'bathrooms,' and 'minimum nights'. For all models, al skewed columns were normalized, and the data was split into 70% training data and 30% test data with a random state of 0.

Each notebook has all the models tested and their corresponding scores are displayed, each model has optimal parameters. All regression models test to see which model can best predict prices whereas all classification models attempt to find a model that can best predict a price range.

Since there were many varibales that could affect price, to avoid overfitting a model dimenbsion reduction techniques were used such as PCA, LDA (only for classification), and Kernel PCA. All techniques were used as there is no single best technique for all ML models. 

To optimize the models grid search and K-fold Cross validatioon were used to find the best possible combionation of parameters. 
