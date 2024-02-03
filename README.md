# Detection_of_insider_threat

**INTRODUCTION:**

Insider threats are a complicated and difficult problem to identify and avoid  because they mostly have privileged access to the network and database of company details. We have trained the model with only the normal behaviour so that the model finds the insider when a user data deviates from the normal behavioural data and this has been already implemented with ML methods like one-class svm, isolation forest etc but we have implemented this method in LSTM.

**DATASET:**

The CSE-CIC-IDS-2018 dataset is a realistic cybersecurity dataset collected by the Canadian Institute for Cybersecurity (CIC) at the University of New Brunswick. It contains network traffic data from a realistic network environment, including normal traffic and various types of attacks. It is available on the Registry of Open Data on AWS, which is a collection of publicly available datasets hosted on Amazon Web Services (AWS). It contains 80 features, including basic flow features (such as duration, packets, bytes), statistical features (such as mean, variance), content features (such as HTTP requests, user agents), and time-based features (such as timestamps, inter-arrival times). The dataset also includes labels indicating whether each network flow is benign or malicious.

**LSTM:**

LSTM (Long Short-Term Memory) is a type of recurrent neural network (RNN) architecture that is widely used for sequential data analysis, such as time series forecasting, natural language processing, speech recognition, and more. Unlike traditional RNNs, which suffer from the vanishing gradient problem and have difficulties in remembering long-term dependencies, LSTMs use a memory cell and several gates (input gate, forget gate, output gate) to control the flow of information and selectively remember or forget previous inputs. LSTMs have been shown to be effective in modelling time series data with long-term dependencies and are often used in anomaly detection, where the goal is to identify patterns in the data that deviate significantly from the expected behavior.

**ISOALTION FOREST:**

Isolation Forest is an anomaly detection algorithm based on the concept of decision trees. It randomly selects a feature and a split value to partition the data into two parts, one with anomalies and one without. It repeats this process until each anomaly is isolated in its own partition, making it an outlier. It does not make any assumptions about the distribution of the data and can handle high-dimensional data efficiently.

**ONE-CLASS SVM:**

One-class SVM is a type of support vector machine that learns a decision boundary around the normal data points in a dataset, with the aim of identifying the anomalies as the points outside the decision boundary. One-class SVM is suitable for unsupervised anomaly detection tasks, where there is no labeled data for training a supervised model.

**ADVANTAGES:**

Our project is implemented with LSTM so it has a memory to store the previous data input with which they can understand the patterns better than then ML models. Another major advantage is that for this project even if an organisation has only the normal user data it is enough to train the model no need of implementing an attack and observing its parameters by providing more amount of normal user data which will be easy for an organisation to get from their network traffic we could identify an insider.

**CONCLUSION:**

Clearly, on comparing isolation forests and one-class SVM with the LSTM, it is observed that the LSTM algorithm has a higher accuracy of 76% than 49% of Isolation Forest and 66% of one-class SVM . Thus, it is seen that for detection of insider threat, the better algorithm is LSTM and the LSTM algorithm performed with the best accuracy on this dataset. It is proved that deep learning method provides more accuracy than machine learning method since deep learning suits for this type of network traffic dataset.

