# <b>A Robust Machine Learning Based System for Identification of Network Intrusions with Data Balancing</b> <div align="center">

Intrusion detection systems' (IDSs) ability to protect company communication is crucial to 
cybersecurity. The reason for this is because intrusion detection systems play a crucial role as 
the initial defence against harmful assaults. Intruder detection using machine learning is becoming increasingly popular, but it still has some limitations that may be efficiently overcome by 
integrating diverse designs. So, this study's goal is to improve an 
efficiency of various IDS machine learning frameworks by addressing these issues through 
the application of data balancing approaches on two prominent datasets, the UNSWNB15 and 
the CIC-IDS-2017.


<b>Task</b>: This study aims to improve the efficacy of a variety of machine learning frameworks for 
intrusion detection systems by addressing issues associated with unbalanced datasets 
through the implementation of data balancing techniques.
<ul>
<li>To gather and examine the UNSW-NB15 andCIC-IDS-2017 intrusion detection datasets after learn more about their structure, feature types, and data distribution.</li>
<li>To guarantee high-quality data, preprocess datasets by standardising values, correctly labelling data, and checking and controlling null values; these steps are essential for building strong ML models.</li>
<li>To fix imbalanced datasets, use data balancing approaches. Then, train various intrusion detection models on the balanced datasets.</li>
<li>To enhance model performance through the use of feature engineering approaches; more particularly, to identify and extract critical features that greatly assist in detecting network intrusions.</li>
<li>To utilise test and train datasets to develop hyperparameter-tuned DL models for NID and classification systems.</li>
<li>To assess an efficacy of the trained models in terms of detection using measures such as ROC curve, recall, accuracy, precision, F1-score, and complexity</li></ul>


<b>Research Question</b>
<ul>
<li>RQ1: What effect do data balancing techniques have on a performance of ML models 
for detecting intrusions in networks when applied to the CIC-IDS-2017 and UNSW
NB15 datasets? </li>
<li>RQ2: How do different machine learning methods enhance the performance of 
intrusion detection on the CIC-IDS-2017 and UNSW-NB15 datasets? </li>
<li>RQ3: What are the comparative strengths and weaknesses of the developed models 
based on various performance metrics such as accuracy, precision, and recall? </li></ul>

<b>Proposed methodology</b>
<ul>
<li>collect publicly available datasets namely the UNSW_NB15 dataset from Kaggle open source and Intrusion detection evaluation dataset (CIC-IDS2017) by the CIC website.</li><li>conduct preprocessing for improve data efficiency. In pre-processing dataset cleaning by checking for and removing null, duplicate, and infinite values, as well as dropping irrelevant columns to reduce noise and complexity. </li><li>Categorical variables are converted to numerical values using label encoding to facilitate model training.</li><li> Data is normalised by standard scaling to maintain uniformity across features, and the SelectKBest approach is used to do feature selection to discover a most influential feature. </li><li>By oversampling the minority class and deleting overlapping occurrences, the SMOTE-ENN approach balances the dataset, addressing an issue of class imbalance. </li><li>The dataset is then split into two sections: 80% of the data is used for the training set, while the remaining 20% is used for the testing set.</li> <li>The study implements advanced machine learning algorithms, including Extra Trees, LSTM, and XGBoost, which are known for their effectiveness in detecting intrusions, to build and evaluate the predictive models. Next, use f1-score, recall, accuracy, and precision to assess the model's performance.</li></ul>

<b>Overview of the dataset</b> 

The CIC-IDS-2017 and UNSW_NB15 dataset were collected from Kaggle, containing both 
normal and attack records. UNSW_NB15 the dataset is structured with a training set of 
175,341 records and a testing set of 82,332 records. While CIC-IDS-2017 includes 2,830,743 
records, categorized into 15 types (one for normal traffic and 14 for various attack types). With 
84 extracted features.

<b>Data pre- processing</b>
<ul><li>Check null values in data</li>
<li>Dropped null values and duplicate values</li>
<li>Check the infinite valuers</li>
<li>Dropped irrelevant columns</li></ul>

<img src="picture2.png" alt="width= 100">

