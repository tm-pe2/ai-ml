## [Anomaly Detection in Machine Learning](#top)

Anomaly detection in machine learning is the process of identifying anomalies or outliers in a dataset. 

- **Anomalies** are unusual data points which are significantly different to the wider trends in the rest of the data set. They are unexpected deviations from the expected outcome. 

- Anomaly detection in machine learning is an important topic because models are so reliant on high quality data. Anomalies or outliers can skew the quality of this training data, as machine learning models are developed to understand the *relationship between data points*. 

- Outliers may affect **the accuracy of the model** by altering patterns learned by the model. 

- Sometimes models can be overfit to training data too, which lowers the model’s ability to generalise when facing new or unseen data. An anomaly in this case may be a sign that the model itself should be retrained, or a data scientist must intervene. For example if a model was trained without a specific subset of demographic data, a relatively normal data point may be flagged as an anomaly if the model encounters a group unrepresented by the training data. In this case the model would need to be retrained to bring into account the bias. 


### Anomaly categories:
 

1. Point Anomaly: A tuple in a dataset is said to be a Point Anomaly if it is far off from the rest of the data.
2. Contextual Anomaly: An observation is a Contextual Anomaly if it is an anomaly because of the context of the observation.
3. Collective Anomaly: A set of data instances help in finding an anomaly.


## Anomaly Detection using the concepts of Machine Learning:
 
 
* **Supervised Anomaly Detection:** This method requires a labeled dataset containing both normal and anomalous samples to construct a predictive model to classify future data points. The most commonly used algorithms for this purpose are *supervised Neural Networks, Support Vector Machine learning, K-Nearest Neighbors Classifier*, etc.

* **Unsupervised Anomaly Detection:** This method requires any training data and instead assumes two things about the data: <br>
1. Only a small percentage of data is anomalous, 
2. Any anomaly is statistically different from the normal samples. <br><br>
Based on the above assumptions, the data is then clustered using a similarity measure and the data points which are far off from the cluster are considered to be anomalies.


