# network_intrusion_detection
# Overview
This project implements a Network Intrusion Detection System (NIDS) using machine learning algorithms to classify network traffic as either normal or anomalous. The dataset used in this project is a CSV file containing various network traffic attributes, and the task is to identify abnormal or malicious behavior within the data.

# Dataset
The dataset consists of network traffic data with the following columns:

duration: Duration of the connection

protocol_type: Type of protocol used (TCP, UDP, etc.)

service: The service used (e.g., HTTP, FTP)

flag: Status of the connection

src_bytes: Number of bytes sent from the source

dst_bytes: Number of bytes sent to the destination

class: Label indicating whether the traffic is normal or anomalous (target variable)

# Libraries and Tools
The following libraries are used in this project:

numpy, pandas: For data manipulation and analysis

matplotlib, seaborn: For data visualization

scikit-learn: For machine learning algorithms and model evaluation

xgboost, lightgbm: For advanced boosting models

tabulate: For formatting output

# Data Preprocessing
Loading Data: The training and test datasets are loaded from CSV files.

Handling Missing Values: Any missing data is handled, although there are no missing values in the dataset.

Label Encoding: Categorical variables like protocol_type, service, and flag are encoded into numerical values using LabelEncoder.

Feature Selection: The num_outbound_cmds column is dropped as it is deemed irrelevant for the classification task.

# Model Building

Several machine learning models are used to classify the network traffic:

Logistic Regression

K-Nearest Neighbors (KNN)

Decision Tree Classifier

Random Forest Classifier

AdaBoost Classifier

Gradient Boosting Classifier

SVC (Support Vector Classifier)

XGBoost Classifier

LightGBM Classifier

The dataset is split into training and testing sets, and the models are trained on the training data and evaluated using accuracy metrics.

# Evaluation

The models are evaluated using metrics like accuracy, precision, recall, and F1 score. The project focuses on detecting malicious network behavior, which can be used in intrusion detection systems to enhance network security.

# Results

The class distribution in the dataset shows a slight imbalance, with more instances of the "normal" class than the "anomaly" class.

The best-performing model can be selected based on the evaluation metrics.

# Conclusion

This project demonstrates the use of machine learning to classify network traffic and detect anomalies. It can serve as a foundation for developing more advanced intrusion detection systems using different datasets and more sophisticated techniques.

# Requirements
Python 3.x

Required libraries: numpy, pandas, scikit-learn, matplotlib, seaborn, xgboost, lightgbm, tabulate
