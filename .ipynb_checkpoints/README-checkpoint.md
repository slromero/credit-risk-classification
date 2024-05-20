# Assignment 20 
# Credit Risk Classification

## Overview of the Analysis

We created a logistic regression model to predict the creditworthiness of potential borrowers, based on a set of known factors that would be known at the time a loan application is submitted. If successful, the model could be used to classify a good loan application versus one that presents a potential risk to the lender.

The current dataset allowed us to apply a supervised learning methodology to construct the model, where we were aware of the ultimate status of each loan (loan status 0: healthy; loan status 1: high-risk, leading to default). This "score" was used to train the model on the characteristics of each score. We ran the model again on a test dataset, also with known scores, in order to assess the model's performance as a predictor of creditworthiness. If effective, the model could help with decision-making regarding new applications.

The data was provided in .csv format and analyzed using python in Jupyter lab, using python modules pandas and numpy, as well as several sklearn modules for machine learning. The dataset was balanced to have the same number of records for each score.  The data then was split into training and testing sets, and the features and target value (loan status) were defined. A standard scale was applied to the numeric data.  The model was run individually on the training set and testing set, respectively, and evaluated via metrics provided by sklearn to determine how well the factors predicted the actual loan status.

The result was examined further to correct for potential overfitting on the particular datasets used, meaning that the result could be dependent on attributes of the current dataset, rather than generalized for expanded use.  Overfitting would make the model less effective for applying to future datasets.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Logistic Regression Model #1
      (Test Dataset)
      Accuracy:  1.00
      Healthy Loan: Precision 1.00, Recall 0.99
      High-Risk Loan: Precision 0.99, Recall 1.00

* KNeighborsClassifier Model #2
      (Test Dataset)
      Accuracy:  1.00
      Healthy Loan: Precision 1.00, Recall 0.99
      High-Risk Loan: Precision 0.99, Recall 1.00

* Logistic Regression Model after Dataset Reduction #3
      (Test Dataset)
      Accuracy:  1.00
      Healthy Loan: Precision 1.00, Recall 0.99
      High-Risk Loan: Precision 0.99, Recall 1.00

* KNeighborsClassifier Model after Dataset Reduction #4
      (Test Dataset)
      Accuracy:  1.00
      Healthy Loan: Precision 1.00, Recall 0.99
      High-Risk Loan: Precision 0.99, Recall 1.00  
  

## Summary

The models selected here did not yield a good result because all results appeared to be subject to overfitting; the results are too good to be true.  

I do not recommend any of these models to determine eligibility for a loan because they do not add anything of value to the current method of approving a loan. Next steps would be to attempt different models using the current features.  It might also be worth considering the addition of new features to the analysis (features not correlated with the current features).