# Multiclass-Classification-of-Customer-Service-Queries

This project is a multiclass classification of customer service queries into seven topics such as "Shipping", "Product Availability", "Returns &amp; Refunds", etc. 

Datset -https://github.com/ARGULASAISURAJ/Multiclass-Classification-of-Customer-Service-Queries/blob/main/Customer_Service_Questions_Multiclass.csv

This corpus contains 5000 customer queries at an online retailer, which are classified into seven topics such as "Shipping", "Product Availability", "Returns & Refunds", etc.

Distribution of Data across topics

![pic2](https://github.com/ARGULASAISURAJ/Multiclass-Classification-of-Customer-Service-Queries/blob/main/Images/pic2.PNG)

**Dataset snapshot**

![pic1](https://github.com/ARGULASAISURAJ/Multiclass-Classification-of-Customer-Service-Queries/blob/main/Images/pic1.PNG)

**Text cleaning procedure**

dropna

remove stopwords and words with length less than 2

removed numerical text

lemmatized words

**Dataset snapshot after cleaning**

![pic3](https://github.com/ARGULASAISURAJ/Multiclass-Classification-of-Customer-Service-Queries/blob/main/Images/pic3.PNG)


Encoded Categories using **Label encoder**.

**Vectorisation technique**

Bag of word vectorisation using TF-IDF.

**Classification models built**

NaiveBayes Classifier

KNN classifier

Random forest classifier

Deep neural network classifier.


**Metrics used for model evaluation**

Classification report-precision,recall,F1-score

Confusion matrix

ROC Curve

Precision recall curve

**Choice of metrics**

Accuracy is not a good metric, because it performs poor on imbalanced dataset. Whereas Precision, recall and F1-score are good metrics for classification even if there is any imbalance representation of predicted class in datset. Classification report gives us thes metics. Confusion matrix gives us visual representation of model performance and comparision between True and predicted classes, Other metrics F1,Precison,recall are calculated from Concusion matrix. AUC-ROC(Area under the curve of reciever characterstic operator) is another metric for classification problems, which is a probability curve that plots True Positive rate aganist False positive rate at various thresholds for each of the Classes. AUC is the ability to measure the ability classifier to distinguish between classes.Also a Summary to ROC.

**Observations**
From the above models(Naive Bayes, Random Forest, K-nearest Neighbour, Deep Neural Network)-
Naive bayes worked best on holdout dataset with weighted avg F1 score of 0.93 compared to Random forest, KNN and DNN with F1 score of 0.92, 0.84, 0.88 respectively.
when it comes to AUC- Naive bayes performed well with an AUC of 0.99 compared to Random forest 0.98, KNN 0.96 and DNN- 0.98
New models implemented-KNN,DNN
