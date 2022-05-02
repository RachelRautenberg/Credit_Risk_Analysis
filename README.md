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
                   ![brf_confusion]()
- Balanced Accuracy: 78.9%
- Classification Report: 
                   ![brf_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/brf_classification.PNG)

##### EasyEnsembleClassifier
- Confusion Matrix: 
                   ![eec_confusion](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/eec_confusion.PNG)
- Balanced Accuracy: 93.2%
- Classification Report: 
                   ![eec_classification](https://github.com/RachelRautenberg/Credit_Risk_Analysis/blob/main/Resources/eec_classification.PNG)
                   
                   
Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
