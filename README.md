
#  Final Project Requirements

## NOTE: Data_Gathering notebook must be run first to aquire data files as Git cannot support such large files in its repositories.

## Introduction

Insurance coverage and mental health have been popular topics in the U.S. as of late. We have been tasked with collecting data on insurance coverage within the U.S. and examining how people utilize it to address mental health pathology. 

The present notebook will explore these relationships via CDC data in addition to developing meethods to identify participant insured status or a recent lack of insurance coverage. 

## Objectives

* explore variable relationships within BRFSS data
* establish health/insurance coverage trends across U.S.
* predict insured status of those with recent mental health sypmtoms
* predict lack of insurance coverage during the previous year based on recent mental health symptoms

## Conclusions

The southeast region of the U.S. has a lower perceived quality of life and higher prevalence of recent mental/physical ailments that affected everyday life. 

Recent mental health problems can be lined to insured status in addition to predicted a lack of insurance in the past 12 months. However, predictive models are not powerful enough to accurately predict insured status or a recent lack of insurace.

Overall, BRFSS data was of a lower quality, making it hard to create acceptably powerful predictive models. Further actions should be taken to improved the quality of data for more robust modeling in the future. 

## Function Clarification

### classifier_generator(y, X, clf_list)

* clf_list needs to be a list of classifiers with random_state uniformally defined. An example is included below:
    * clf_list = [XGBClassifier(random_state=0), LogisticRegression(random_state=0), 
            AdaBoostClassifier(random_state=0), GradientBoostingClassifier(random_state=0)]
* train-test-split is included in the function. 
* random_state needs to be the same across classifiers for uniformity across classifiers

### Data_Cleaning: on_the_bubble

*The comment out boxes are code used to customize the questions you want to focus on within the BRFSS data sets.
    * Feel free to remove or optimize this code as you see fit. 

## Packages Needed

* numpy
* pandas
* seaborn
* matplotlib.pyplot
* folium
* warnings
* statsmodels.api
* sklearn.pipeline
* sklearn.model_selection 
    train_test_split
    GridSearchCV
* sklearn.linear_model
        LogisticRegression
* sklearn.ensemble
    RandomForestClassifier
    GradientBoostingClassifier
    AdaBoostClassifier
* sklearn.metrics
    accuracy_score
    classification_report
* xgboost
    XGBClassifier
* yellowbrick.classifier 
    ConfusionMatrix
* imblearn.over_sampling
    SMOTE

## Deliverables

* slide deck (BRFSS Psychopathology and Insurance)
* audio/visual walkthrough (https://drive.google.com/open?id=1YJX1PsgEvbYVLGlyRF2OLoT1w7F_c_Yj)
* technical blog
* Data_Cleaning notebook
* Data_Gathering notebook
* EDA_and_Classification notebook

## Blog Post Link
https://neji128.github.io/under_construction
