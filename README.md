# Credit Risk Analysis
## Overivew

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, a dataset will be oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling will be done using the SMOTEENN algorithm. Next, two new machine learning models that reduce bias will be compared, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Lastly, an evaluation of the performance of these models will be made on whether they should be used to predict credit risk.

Software used included Python 3.7.9, Anaconda 4.9.2, and Jupyter Notebooks 6.1.4.

## Results
### Resampling Models
#### Oversampling: RandomOverSampler

![mod17_1](https://user-images.githubusercontent.com/10467547/166126128-7dd96ae1-0070-4c46-a2bf-b37528c6ab95.png)

Balanced Accuracy Score: 65.7%

High-risk Precision Rate: 1%
High-risk Recall: 60%
F1: 2%

Low-risk Precision Rate: 100%
Low-risk Recall: 71%
F1: 75%

#### Oversampling: SMOTE

![mod17_2](https://user-images.githubusercontent.com/10467547/166126147-fca083f2-0427-496d-afd1-efe5683a9e5c.png)

Balanced Accuracy Score: 66.2%

High-risk Precision Rate: 1%
High-risk Recall: 63%
F1: 2%

Low-risk Precision Rate: 100%
Low-risk Recall: 69%
F1: 82%

#### Undersampling: ClusterCentroids

![mod17_3](https://user-images.githubusercontent.com/10467547/166126151-d221119f-c178-445e-b0c9-350d9194a242.png)

Balanced Accuracy Score: 54.4%

High-risk Precision Rate: 1%
High-risk Recall: 69%
F1: 1%

Low-risk Precision Rate: 100%
Low-risk Recall: 40%
F1: 57%

### SMOTEENN Algorithm
#### Combination Sampling

![mod17_4](https://user-images.githubusercontent.com/10467547/166126172-7a5957dd-e291-427b-a215-69d6e50d1f7a.png)

Balanced Accuracy Score: 64.4%

High-risk Precision Rate: 1%
High-risk Recall: 72%
F1: 2%

Low-risk Precision Rate: 100%
Low-risk Recall: 57%
F1: 72%

### Ensemble Classifier
#### Balanced Random Foest Classifier

![mod17_5](https://user-images.githubusercontent.com/10467547/166126178-f02a48df-5fd4-471a-9ef3-6e267025296c.png)

Balanced Accuracy Score: 78.9%

High-risk Precision Rate: 3%
High-risk Recall: 70%
F1: 6%

Low-risk Precision Rate: 100%
Low-risk Recall: 70%
F1: 93%

#### Easy Ensemble Classifier

![mod17_6](https://user-images.githubusercontent.com/10467547/166126186-d9dc326d-6e6d-4af9-865d-bc127e4c7ce3.png)

Balanced Accuracy Score: 93.2%

High-risk Precision Rate: 9%
High-risk Recall: 92%
F1: 16%

Low-risk Precision Rate: 100%
Low-risk Recall: 94%
F1: 97%


## Summary

Out of all six models, the EasyEnsembleClassifer model yielded the best results, and is the one I would recommend. For high-risk candidate prediction, the accurary rate of this model was 93.2%, precision rate was 9%, sensitivity rate (recall) was 92%, and F1 was 16%. For the low-risk candidate prediction, the sensitivity rate was 94%, and the F1 score was 97%.
