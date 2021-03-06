# Credit_Risk_Analysis
Module 17

## OVERVIEW OF ANALYSIS
Overview of the analysis: Explain the purpose of this analysis.

Determining credit risk can present a challenge due the the nature of the business with the number of good loans far outweighing those that are risky. 

After learning a variety of techniques when working with imbalanced data, those skill are put to use to help a dear friend, Jill, determine a model that will most benefit the company going forward to evaluate credit risk.  The tools that will be utilized for this analysis are:
  * RandomOverSampler
  * SMOTE
  * ClusterCentroids
  * SMOTEENN
  * BalancedRandomForestClassifier
  * EasyEnsembleClassifier

Once the analysis is complete, we will wrap up the full presentation with a recommendation, or justification for no recommendation, based on the performance of the various models to predict credit risk. 


## RESULTS OF MODELS
##### Random Over Sampler 
- Confusion Matrix: 

     ![ros_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/ros_confusion.PNG)
- Balanced Accuracy: 65.7%
- Classification Report: 

     ![ros_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/ros_classification.PNG)
                   
##### SMOTE Oversampling
- Confusion Matrix: 

     ![smote_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/smote_confusion.PNG)
- Balanced Accuracy: 66.2%
- Classification Report: 

     ![smote_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/smote_classification.PNG)
                   
##### ClusterCentroid Undersampling
- Confusion Matrix: 

     ![cc_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/cc_confusion.PNG)
- Balanced Accuracy: 54.4%
- Classification Report: 

     ![cc_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/cc_classification.PNG)
                   
##### SMOTEENN Combination Sampling
- Confusion Matrix:

     ![smoteenn_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/smoteenn_confusion.PNG)
- Balanced Accuracy: 68.8%
- Classification Report:

     ![smoteenn_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/smoteenn_classification.PNG)

##### BalancedRandomForestClassifier
- Confusion Matrix:

     ![brf_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/brf_confusion2.PNG)
- Balanced Accuracy: 78.9%
- Classification Report:

     ![brf_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/brf_classification.PNG)

##### EasyEnsembleClassifier
- Confusion Matrix:

     ![eec_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/eec_confusion.PNG)
- Balanced Accuracy: 93.2%
- Classification Report:

     ![eec_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/eec_classification.PNG)
                   
                   
## Summary
To evaluate which of these models will work best for the purpose of evaluating credit risk, we need to look at several things, let???s start with accuracy. The ClusterCentrod Undersampling model can be removed as a contender simply by looking at accuracy. The accuracy of the ClusterCentroid is barely over 50%, I simply would not recommend based off of that.  Precision and recall would not change this.  There are several models with accuracy in the mid to high 60s.  If these models were the final options, use of them would come with the recommendation to explore deeper.   For example, review importance of features, the reduce data features to narrow the working data for the machine to better learn and predict. 

Lucky for us there were two models that resulted in accuracy higher that 75%.  Looking at the EasyEnsembleClassifier, which resulted in 93.2% accuracy, the next steps of evaluation can be taken.  Before moving on, it is good to address the underlying concern that such high accuracy is the result of an overfit model.  We can safely say that is not the case here as the same data was run with no additional cleaning for each of the predictive models used.  The f1 score for the EasyEnsembleClassifier is .93 which would suggest that a very good balance of both precision and sensitivity was achieved.  This model produced the lowest number of false negatives, which is also evident in the recall score of .92. Finally, the EasyEnsembleClassifier had the highest precision rate for catching high risk potential. All models achieved perfection for predicting low risk, which would be expected with the imbalanced data, but is not an important factor with the scenario of looking for high risk.
