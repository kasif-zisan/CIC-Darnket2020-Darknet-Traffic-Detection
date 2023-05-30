# CIC-Darnket2020 Darknet Traffic Detection Model

## Introduction

This repository presents an analysis of the CIC-Darknet2020 dataset and the use of supervised classification models to classify network traffic flows. Initially, we analyzed the data and cleaned it before preprocessing it for the use in two machine learning models: Decision Tree Classifier and Logistic Regression.

In this repository, we showed the steps we took for data observation, cleaning, visualization, preprocessing and applying them in Machine Learning Models.

After conducting result analysis, we observed that Decision Tree Classifier performed better than Logistic Regression in the classification of network flows.


## Dataset Description

The CIC-Darknet2020 dataset, created by the Canadian Institute for Cybersecurity (CIC), is a comprehensive dataset created for research and development of methods for detecting and analyzing darknet traffic.


The dataset consists of both darknet and benign traffic. The first layer generates the traffic types - Tor, Non-Tor, VPN, NonVPN. The second layer of the dataset consists of Audio-Streaming, Browsing, Chat, Email, P2P, File-Transfer, Video-Streaming, and VOIP. The CIC-Darknet2020 dataset provides a variety of features extracted from the network traffic data, such as Average Packet Size, Average Packet Length, Flow IAT Mean, Flag Counts - PSH, FIN, SYN etc., Flow Duration, Source and Destination IP addresses, Source and Destination Ports, Protocol types, and other relevant information.


The dataset includes two labels for each data point, one is from the first layer which represents the type of network flow and the other is from second layer representing the data that is being sent.


The Darknet dataset comprises a total of 141,530 records, including 118,611 benign samples and 22,919 darknet samples. The dataset has 85 features in total.

Here are some basic information about the dataset -
* The shape of the dataset is - (141530, 85). It means that the dataset has 141530 rows and 85 features.
* RangeIndex: 141530 entries, 0 to 141529
* All the features have 141530 non-null values, but Flow Bytes/s feature has 141483 non-null values meaning there are missing values in Flow Bytes/s feature.
* The datatypes are - int64(55), float64(24) and object (6). As a result of using 64-bit data type variables, the dataset is using up more memory.
* Total memory usage is 91.8+ MB.
* We also see that 83.8% of the dataset contains Benign traffic flow data points and 16.2% of the dataset contains Darknet traffic flow data points. This means that the dataset is imbalanced.


**The detailed model and parameter description and performance measure, evaluation and comparison are in the notebook.**




