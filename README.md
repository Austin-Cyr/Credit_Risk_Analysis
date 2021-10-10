# Credit_Risk_Analysis

## Overview of the Analysis: 

Many datasets encountered in the world are inbalanced. This can create a challenge for developing models that are both accurate, precise and do not overfit the trained data. For this project, we are tasked with creating and testing 6 different models. Once created, we evaluated each on their performance to meansure and predict credit risk, which is inherently imbalanced. 

We utilized multiple methods and algorithms to review the data and results from different perspectives. We first oversampled the data with the RandomOverSamnpler and SMOTE algorithms. Then we undersampled the data with the ClusterCentroids algorithm. After which, we tried the SMOTEEN algorithm which over and undersampled simultaneously. And then finally, we looked at two ensemble models that reduce bias, BalancedRandomForestClassifer and EasyEnsembleClassifier. 

## Results:

### Oversampling
  #### RandomoverSampler
    - Balanced Accuracy: .65
    - Precision: .01
    - Recall: .73
  ![image](https://user-images.githubusercontent.com/84824391/136682719-caf6abb5-d544-4039-994a-d26ab3f4c0cb.png)


  #### SMOTE
    - Balanced Accuracy: .66
    - Precision: .01
    - Recall: .63
   ![image](https://user-images.githubusercontent.com/84824391/136682708-9b575e0b-e8eb-497f-b573-36ee6f796a73.png)

### Undersampling
  #### ClusterCentroids
    - Balanced Accuracy: .54
    - Precision: .01
    - Recall: .69
   ![image](https://user-images.githubusercontent.com/84824391/136682700-716dda3f-4633-46b4-ae48-e6cd89412291.png)

### Combinatorial -Over and -Under Sampling
  #### SMOTEEN
    - Balanced Accuracy: .65
    - Precision: .01
    - Recall: .72
  ![image](https://user-images.githubusercontent.com/84824391/136682687-ba7523ad-d354-4735-a1cf-27cf04b099ce.png)

### Ensemble Models
  #### BalancedRandomForestClassifier
    - Balanced Accuracy: .96
    - Precision: .77
    - Recall: .93
   ![image](https://user-images.githubusercontent.com/84824391/136682733-ceebfc7a-1b61-40f3-a439-43f71b579314.png)


  #### EasyEnsembleClassifier
    - Balanced Accuracy: 1.0
    - Precision: 1.0
    - Recall: 1.0 
   ![image](https://user-images.githubusercontent.com/84824391/136682729-60e0e2b1-022a-4289-ae50-90f5c6baa9ac.png)

   
## Summary:

Predicting credit risk is a challenging task, considering that the known data is naturally imbalanced. While there are methods to control for this, each method is not necessarily perfect. After reviewing each of the model's results from their training and predicted results, one model stands out as the best to fit this type of purpose and data set, the BalancedRandomForestClassifier. This model not only has a high Balanced Accuracy of .96, but also a high Recall of .93. While it's precision is in the high 70's, this is substantially better then the rest. While the EasyEnsembleClassifier may seem a good fit, since its numbers were 1, 1, and 1, this also leads me to believe that an issue arose in the model creation or it will overfit future datasets and not serve its purpose. 
