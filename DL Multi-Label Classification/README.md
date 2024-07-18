# DL Multi-Label Classification

In this section I tried to predict multi-label classification with Feed-Forward Neural Network

I decided to use Feed-Forward Neural Network because it's easy to implement and can get good results

I started by splitting the data into features (X) and target (y)

I scaled my features with RobustScaler because they are wide scattered and encoded the categorical labels

I splitted the data into train and test

I chose to use a simple FF NN with three hiden layers. First layesr at the size of 64, second at the size of 32 and last at the size of 16

In real life I would try different architectures for that network with different sizes and number of layers 

In the model evaluation I can see that it performed well on some labels and poorely on others

It done well on classes with large semple size and bad on small ones

To improve the model perfoemance I can try use deifferent features, different model architectures, train the model on more semples and try different hyper parameters
