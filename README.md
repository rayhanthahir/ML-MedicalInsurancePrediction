# ML-MedicalInsurancePrediction

Dataset: https://www.kaggle.com/datasets/harishkumardatalab/medical-insurance-price-prediction 

This repository contain my personal project which mainly purposed to predict medical insurance price based on several variable which can effect the medical insurance price

## Data Understanding
The dataset contains 7 column include:
1. Age
2. Sex
3. BMI (Body Mass Index)
4. Children
5. Smoker
6. Region
7. Charges

Based on EDA and data analysis, i decide to drop Children column/attribute because it seems irrelevant to the current problem

## Preprocessing
Before jump into modelling, first we need to preprocess the data. I used Label Encoder and One Hot Encoding for change categorical value into numerical value. Next, i handle the oultlier from the data by using its median value based on the smoker attribute value. If the smoker attribute value is 1 (the patient has smoked before) the outlier value will be replaced by charges attribute median value when the attribute value is 1, vice versa will be applied to smoker attribute value is 0. Then, i used standard scaler to scale the training and test variable.

## Modelling
I used 4 mahine learning algorithm including linear regression, decision tree, random forest, and Bayesian bayesian ridge. Based on the result, decision tree get the based result.
Mae Decision Tree:  440.51430087087084
RMSE Decision Tree: 2067.1266657600204


