# Enron_email_classification
This is a classification project on the Enron Email Dataset. The dataset is the May 7, 2015 Version of dataset, as published at https://www.cs.cmu.edu/~./enron/. The project was undertaken as part of Post Graduate Diploma Program of IIIT Hyderabad organized by Talent Sprint. The project was jointly carried out by Somasundaram Chidambaram and Vinod Thomas.

# Enron_data_download.ipynb
This downloads the data and saves as a csv file.

# Enron_KMeans_final.ipynb
This is an attempt to classify the emails unsupervised based on the natural structure of the data. Eventually 23 clusters were identified, but these were not clearly segregated. Hence further exploration on these lines was dropped. A TSNE plot showing the relative positions of the classes was generated. 

# Tfidf_Enron_final.ipynb
The text data was vectorized using Tfidf and concatenated with the other features. Various machine learing algorithms were applied on the resulting vector. The test accuracies obtained were as follows:
KNN 0.64
Random Forest 0.69
Gradient Descent 0.81
SVC 0.80
LR 0.88

# LSTM_Enron_final_ver2.ipynb
LSTM was applied on the text data and the same was concatenated with the other categorical data. The resulting accuracy on the test sample was 0.71


# Enron_bert_13.ipynb
Bert was applied on the text data. The bert embedding concatenated with the other categorical data was classified using a simple 3 layer MLP classifier. The results were not highly accurate. Further work needs to be done on this.

# Enron_Deployment.ipynb
This is the model that was deployed. The text data is vectroized using tfidf, and the categorical data were concatenated. The resulting vector was classified using Logistic Regression, to arrive at test accuracy of 0.86


