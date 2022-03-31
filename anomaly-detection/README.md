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


## Anomaly Detection Techniques in Python

These techniques identify anomalies (outliers) in a more mathematical way than just making a scatterplot or histogram and eyeballing it. If a point is an outlier with respect to its values across 30 features (a multivariate outlier), not possible to identify it using the above methods, which is where these techniques come in.

### Definitions:

- An <ins>__outlier__</ins> is an observation with at least one variable having an unusual value.
- A <ins>**univariate outlier**</ins> is an observation with a variable that has an unusual value.
- A <ins>**multivariate outlier**</ins> is an observation with at least two variables having unusual values.


## What Is an Anomaly?
Let's start the review with the 'anomaly' definition. An anomaly is a value that deviates from the norm considerably enough to be regarded as a rare exception. Systems detecting anomalies do that based on the assumption that such outliers, or exceptions, should stand apart from the significant portion of data in the dataset. Thus, the process of detection presupposes the establishment of patterns first and then identifying the units violating those patterns.

Thus, in line with the description provided above, one may derive the 'anomalous' definition as the one that doesn't fit the norm, that is, the expectations of normal behavior or normal value typical for a specific dataset. The unit of data may be too large or too small compared to the major portion of the data, thus deviating from the average values. If the dataset is visualized, an anomalous data unit will stand far apart from the densely placed rest of the data units.

However, in practice, anomaly detection is still challenging, as in most cases, the meaning of anomalies is ambiguous. An anomaly from any perspective (a unit considerably different from the dataset) is usually termed a global anomaly. It is easily identifiable, both automatically and manually. But the problem arises with local anomalies (values different from the primary dataset insignificantly) or micro-clusters of deviant data standing quite close to the general dataset. These ambiguities suggest that a more sensitive way of detecting anomalies is via their scoring in terms of anomaly intensity rather than assigning one of the two labels – normal versus anomalous.
product recommendations using ai
## Why Is it Important to Detect Anomalies?
To embrace the significance of anomaly detection in modern information systems and information security, one should answer a question, what does it mean to be an anomaly? Overall, a standard system functions within some predetermined limitations, with all incoming and outgoing data fitting a range of values typical for it. Thus, when individual deviations from the typical expectations are identified, they always serve as red flags for the security personnel and analysts.

### Some areas in which anomaly detection is popular include:

Fraud detection (insurance, banking)
intrusion detection (computer networks, national surveillance)
medical informatics (diagnosis, disorder detection)
fault/damage detection (commerce, industry)

In a nutshell, detecting anomalous data within a system means that something goes wrong. For instance, if all buyers of an e-shop pay $100 on average for a pair of shoes, and some client pays $1,000 for the same purchase, it is an anomaly meaning that either there is a problem with the client's bank or some glitch occurred in the merchant's system. Similarly, if an insurer receives an average MRI check for $300-400 from patients and suddenly gets a $550 check for the same procedure, it should be an alert about a potentially fraudulent transaction requiring a closer investigation.

Another example is the significance of anomaly detection in a computer network. If some anomalous traffic patterns are identified in it, this could be a sign of sensitive data leakage from a hacked computer. Anomalies in the nervous signal transmission on the MRI scan may be a sign of some serious degenerative disease. At the same time, bizarre purchases and cashing activities with a client's credit card may be an alert of the card's theft.

Thus, as one can see, anomaly detection is helpful in many industries and fields, helping specialists identify deviations from the norm to investigate them closer and determine the cause of such deviation. The core to successful detection practices in any organization is to define 'anomalous' for their own datasets, to set specific detection signals for the analytical systems, and to feed in the feedback about correct/incorrect anomaly labeling for the system to learn.
Anomaly Detection Use Cases.
As anomalies in information systems most often suggest some security breaches or violations, anomaly detection has been applied in a variety of industries for advancing the IT safety and detect potential abuse or attacks. Here is a couple of use cases showing how anomaly detection is applied.

### Cyber-intrusion
Cyber-security is usually guaranteed with the help of network behavior anomaly detection (NBAD) technology. The system analyzes packet signatures to detect security threats and block incoming/outgoing data that is compromised. NBAD also conducts continuous network monitoring to detect suspicious events or trends

### Fraud
Graph-based anomaly detection (GBAD) is used to prevent fraud with credit cards, bank accounts, and insurance. ML systems also enable online banking fraud with the help of behavioral biometrics that also detects anomalies in consumer spending in real-time.

### Medical anomaly detection
Outlier identification has been applied in clinical settings in a variety of ways. For instance, the density-based clustering method can be applied to patient careflow log analysis to see whether the particular patient's careflow trace is anomalous. Anomaly detection in medical image analysis is helpful in accurate diagnostics, while treatment plan analysis may help determine potentially fatal errors in the treatment plans.

### Industrial damage
In the conditions of industrial automation, anomaly detection systems use data coming from numerous sensors to identify any malfunctions in the machinery, thus able to detect abnormalities early to prevent further damage or manufacturing defects.

### Image processing
The ability of anomaly detection systems to compare and analyze images allows accurate fraud detection in banking and insurance (when one recipient of a service submits duplicate reimbursement claims or when fraudsters try to receive reimbursement on fake claims)

### Stock trading
Anomaly detection algorithms deal quite well with the big masses of unstructured data in the stock exchanges, be it regular stocks or cryptocurrencies. ML systems classify the available data about price movements and sales volumes to detect anomalies and give alerts to the users about price outliers. This information may be instrumental in trading decision-making.


## Anomaly Detection with Machine Learning.
Machine learning (ML), an area of artificial intelligence (AI), has proven highly helpful for advancing the anomaly detection accuracy and helping companies and organizations manage big data. The ability of ML systems to learn by their own experience, thus refining their analytical and predictive capacity on their own, is a valuable feature for accurate anomaly detection.

So, what is an advantage of the anomaly detection method enriched with ML technology? The first undeniable benefit is the ML system's ability to handle unlabeled and unstructured data proactively, determining what is normal and what may be regarded as a data anomaly. Second, ML systems are much more sensitive to distinguishing data anomalies from noise, allowing them to differentiate data units based on the degree of their deviation from the norm.