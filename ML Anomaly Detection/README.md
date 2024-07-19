# Anomaly Detection 

In this section, I tried to find anomalies in the dataset using Isolation Forest

I decided to use Isolation Forest because it usually gives good results for anomaly detection and is easy to understand

I started by encoding my labels into 1 for regular communication ('BENIGN') and -1 for all the rest 

Then splitting the data to features (X) and target (y_encoded)

I scale my features with RobustScaler because they are scattered wide

I calculated the contamination of the data to find the scale of anomalies

I built the Isolation Forest model and trained it on the data

Lastly, I predicted the anomalies in the data and evaluated the results

we can see that the results are OK. The model managed to find the anomalies with 66% accuracy

I decided to use all the available features, maybe with a better feature selection I could have reached better results

Also, running the model with different hyperparameters could reach better results

Or maybe the data isn't suited for anomaly detection, there are many different attacks and maybe the ratio of contamination doesn't count as an anomaly and we need different methods
