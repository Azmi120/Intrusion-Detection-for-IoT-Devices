An intrusion detection system (IDS) is a security mechanism designed to monitor and identify unauthorized or suspicious activities within a computer network.

In this project, we are enhancing the system's capabilities through feature engineering of network traffic flow. Our objective is to improve both the accuracy and recall rates in detecting whether activities within the network flow are benign or malicious.

We used Bot-IoT dataset as our network flow data. The dataset is can be found from here: https://ieee-dataport.org/documents/bot-iot-dataset.

## Data Preprocessing

We first visualized the distribution of our data. The data was imbalanced accross the category and sub-category of benign and malicious attacks. We did an undersampling and oversampling to tackle the problem of data distribution.

The code can be found in pre-processing.py

## Feature Engineering
We applied Principal Component Analysis (PCA) and Normalized Gain for the best feature selections. The code can be found in pca.ipynb.

## Baseline Model
initial-ml.ipynb: This notebook reads the data, resamples the categories and chooses the selected features from the feature engineering phase.
We use Decision Tree, Naive Bayes, K-Nearest Neighbors, Logistic Regression, Random Forest, Gradient Boost, Support Vector Machine, ANN, RNN as our baseline model.
We evaluated the accuracy, precision, recall, time taken as our performance metrics.

## Proposed Multi Task learning Model
mlt-bot-iot.ipynb

The model architecture can be found <img src="[https://github.com/user/repo/blob/main/output.jpg](https://github.com/Azmi120/Intrusion-Detection-for-IoT-Devices/blob/main/Multi-task%20Model%20Architecture)" align="center" height="350" width="600"/>


