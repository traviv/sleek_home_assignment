# Feature Importance and Multi-Label Classifier with XGboost

In this section, I decided to use XGboost model to make multi-label classification and use it to find feature importance

I started by splitting my data into features (X) and target (y)

filling NaN values with -1 in the features and scaling them with RobustScaler because they are scattered wide

I encoded the categorical labels with OneHotEncoder and split the data into training and testing

I built the xgboost model and created a multi-class model based on it using MultiOutputClassifier

I trained the model on the training set and predicted on the testing set

In the matrix evaluation, we can see that the model performed very well, maybe too well. 

when seeing the results it immediately causes fear of overfitting, but using an ensemble model like xgboost and different data for training and testing should protect us from it

I could have used another methods to make sure the model wasn't overfitting like k-fold cross-validation

I used the built-in feature_importances to calculate the 10 most important features

5 out of the 10 features are in the backward direction meaning the response from the server helps the classifier more than the ones from the client
