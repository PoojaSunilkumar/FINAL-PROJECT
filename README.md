# <b>A Robust Machine Learning Based System for Identification of Network Intrusions with Data Balancing</b> <div align="center">

Intrusion detection systems' (IDSs) using machine learning is becoming increasingly popular, but it still has some limitations that may be efficiently overcome by 
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

<b>Proposed algorithm</b>

|Algorithm 1: Intrusion detection system                                                                         |
|----------------------------------------------------------------------------------------------------------------|
|strategy                                                                                                        |
|1.	Start                                                                                                        |
|2.	 Collect the publicly available UNSW_NB15 and CIC-IDS2017 datasets.                                          |
|3.	Data Pre-processing.                                                                                         |
|4.	Convert categorical variables to numerical values using label encoding.                                      |
|5.	Apply the SelectKBest technique for feature selection.                                                       |
|6.	Normalize the dataset using standard scaling                                                                 |
|7.	Apply the SMOTE-ENN technique to handle class imbalance by oversampling the minority class and using Edited Nearest Neighbors to clean the data.                                                                             |
|8.	Split the dataset into training and testing sets, with 80:20 ratio.                                          |
|9.	 Select machine learning models like.                                                                        |
|a)	Extra Trees                            |
|b)	LSTM (Long Short-Term Memory)          |
|c)	XGBoost (Extreme Gradient Boosting)    |
|10.	Train each selected model on the training dataset.                                                         |
|11.	Apply the F1-score, recall, accuracy, and precision measures to the testing dataset to assess each model's performance.                                                                                                     |
|12.	stop.                                                                                                      |

<b>Performance Measure</b>

This research assessed the efficacy of XGBoost and LSTM classifiers trained using ML for detecting network intrusions using a number of performance measures, like confusion matrix, AUC, f1-score, recall, accuracy, and precision. To comprehend these factors, a quick summary is given in the next section.

<b>Results of Proposed Models </b>

<ul><li>UNSW_NB15Dataset based on ML models (XGBoost, LSTM and Extra Tree) for network intrusion detection. A performance of a proposed models on the UNSW_NB15dataset reveals that LSTM achieves the best results, with Accuracy92.21%, Precision92.25%, Recall92.21%, and F1-score91.87%, highlighting its superior capability for detecting network intrusions in this dataset.</li>
<li>CIC-IDS-2017Dataset, which relies on ML models for detecting intrusions in networks, are shown in table 4.2. After comparing the suggested models' performance on the CIC-IDS-2017dataset, it is clear that an Extra Tree model is the most reliable IDS, with the greatest F1-score, Accuracy, Precision, and Recall at 99.31%. An XGBoost andLSTM models also performed well.</li></ul>

<b>Conclusion</b>

This paper presents an approach for ML-IDS design using enhanced preprocessing, class weighting, and fine-tuning, tested on UNSW_NB15 and CIC-IDS-2017 to address high-dimensional data and class imbalance. SMOTE-ENN and SelectKBest improved rare intrusion detection, outperforming CNN in imbalanced scenarios.
