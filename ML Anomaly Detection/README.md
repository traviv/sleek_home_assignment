# Anomaly Detection 

In this section, I tried to find anomalies in the dataset using Isolation Forest

I decided to use Isolation Forest because it usually gives good results for anomaly detection and is easy to understand

I started by encoding my labels into 1 for regular communication ('BENIGN') and -1 for all the rest 

Then splitting the data to features (X) and target (y_encoded)

I scaled my features with RobustScaler because they are wide scattered 

I calculated the contamination of the data in order to find the scale of anomalies

I build the Isoletion Forest model and trained it on the data

Lastly I predict the anomalies in the data and evalueted the results

we can see that the results are OK. The model managed to find the anomalies with 66% accuracy

I decided to use all the availble features maybe with better feature selection i could have reach better results

Also by running the model with different hyper parameters could get better results as well

Or maybe the data isn't suited for anomaly detection, there are many different attacks and maybe the ration of contamination doesn't count as anomaly and we need different methods

