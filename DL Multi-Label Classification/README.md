# DL Multi-Label Classification

In this section, I tried to predict multi-label classification with Feed-Forward Neural Network

I decided to use Feed-Forward Neural Network because it's easy to implement and can get good results

I started by splitting the data into features (X) and target (y)

I scaled my features with RobustScaler because they are wide scattered and encoded the categorical labels

I splitted the data into train and test

I chose to use a simple FF NN with three hidden layers. The first layer at the size of 64, the second at the size of 32, and last at the size of 16

In real life, I would try to improve the network by using different architectures with various layers sizes and numbers

In the model evaluation, I can see that it performed well on some labels and poorly on others

It did well in classes with large sample sizes and badly in small ones

To improve the model performance I can try to use different features, and other model architectures, train the model on more samples, and try different hyperparameters
