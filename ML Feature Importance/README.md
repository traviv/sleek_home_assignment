# Feature Importance and Multi-Label Classifier with XGboost

In this section I decided to use XGboost model to make multi-label classification and use it to find feature importance

I started by splitting my data into features (X) and target (y)

filling nan values with -1 in the features and scaling them with RobustScaler because they are wide scattered 

I encoded the categorical labels with OneHotEncoder and splitted the data into train and test

I build the xgboost model and created multi-class model based on it using MultiOutputClassifier

I trained the model on the training set and predicted the testing set

In the matrix evaluation we can see that the model performed very well, maybe too well. 

when seeing the results it immediately causes fear of overfitting, but using ensemble model like xgboost and a different data for training and testing should protect us from it

I could have used another methods to make sure the model wasn't overfitting like k-fold cross-validation

I used the build-in feature_importances to calculate the 10 most important features

