
#  Abstract

## Problem

Insurance coverage and mental health have been a huge top in the U.S. as of late. Our team has been tasked with 

## Methodology

* Data was scraped fron the CDC's BRFSS via a combination of Socrate and request API's
* Logistical regressions were used to explore the relationship between:
    * mental health factors and insured status (insured vs uninsured)
    * mental health factors and a recent lack of insurance during the past 12 months
* A suite of classifiers were utilized to identify an optimal classifier for subsequent hyperparameter tuning.
    This suite included:
        * LogisticRegression
        * XGBClassifier
        * AdaBoostClassifier
        * GradientBoostingClassifier

## Findings

* The southeast portion of the U.S. has a lower perceived quality of life relative to the rest of the U.S. 
* Some regions of the U.S. despite having higher levels of perceived health, experience recent physical and/or mental difficulties that interfere with everyday life.
* Recent bouts with mental health can be used to predict insured status.
* Recent bouts with mental health can also predict lack of insurance coverage in the past 12 months. 
* The predictive models generated small increases in predictive power. Low data quality limited the potential of the classification models.

## Recommendations 

* Transition BRFSS to an online format
    * provides more perceived anonymity increasing the possibility of honest and complete responses
* Incentivize response
    * tax credit of $50 to $100
        * may increase participant pool
        * additional research to gauge the need and feasiblity of an incentive should be done
* Complete an examination of disparities between perceived general health in relation to recent physical/mental health issues