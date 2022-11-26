# Health-Insurance-Charges-prediction-with-Regression
This Repository is for prediction of health insurances charges with regression, submitted for the final assignment of IBM Machine Learning Course 2 (Supervised Machine Learning: Regression).


## Instructions

In this Assignment, you will demonstrate the data regression skills you have learned by completing this course. You are expected to leverage a wide variety of tools, but also this report should focus on present findings, insights, and next steps. You may include some visuals from your code output, but this report is intended as a summary of your findings, not as a code review.

The grading will center around 5 main points:

1.  Does the report include a section describing the data?
2.  Does the report include a paragraph detailing the main objective(s) of this analysis?
3.  Does the report include a section with variations of linear regression models and specifies which one is the model that best suits the main objective(s) of this analysis.
4.  Does the report include a clear and well-presented section with key findings related to the main objective(s) of the analysis?
5.  Does the report highlight possible flaws in the model and a plan of action to revisit this analysis with additional data or different predictive modeling techniques?



## About the Dataset
This dataset was gotten from kaggle, the dataset is has various features that can be used to predict health insurance of individuals. Below are the summary of the columns.

Columns:

1. age: age of primary beneficiary
2. sex: insurance contractor gender, female, male
3. bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height
4. objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9
5. children: Number of children covered by health insurance / Number of dependents
6. smoker: Whether beneficiary is smoking or not
7. region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.
8. charges: Individual medical costs billed by health insurance



## Objective:
The main objective of this analysis is to predict personal health insurance charges of individuals based on their features. other objectives of this analysis include the following;

1. To explore relationships of the various features.
2. To know the key determinant features for insurance charges
3. To know the correlation between insurance charges and other features.


## Summary and Insights:
From the three regression models, the following insights can be drawn:
1. The Linear regression has the R_score for the training set is 75% while the testing score is 74% without any polynomial or regularization features added. The visualization of the actual values vs the predicted values shows that the predicted values is slighly more than the actual values and the model is not well fitted.

2. The Ridge regression without polynomial feature training set R_score is 74%, while the testing score is also 74% compare to the linear regression score this is slightly worse. The visualization of the actual values vs the predicted values shows that the model slightly overfit. The Ridge regression with the polynomial feature training set R_score is 84% and the testing set is 80% compare to the linear regression and the ridge regression without polynomial features, the score is better. The visualization of the actual values vs predicted values show that the predicted values fitted the actual values better than the linear regression and ridge regression without polynomial features.

3. The Lasso regression without polynomial feature training set R_score is 74%, while the testing score is also 74% compare to the linear regression score this is slightly worse, however it is same with the Ridge regression without polynomial features. The visualization of the actual values vs the predicted values shows that the model slightly overfit. The Lasso regression with the polynomial feature training set R_score is 84% and the testing set is 80% compare to the linear regression and the ridge regression without polynomial features, the score is better. However, compare to the ridge regression with polynomial features the score is slighly worse. The visualization of the actual values vs predicted values show that the predicted values fitted the actual values better than the linear regression, ridge regression without polynomial features, and lasso regression without polynomial features, but slighly worse compare to the ridge regression with polynomial features


## Key findings:
1. The dataset do well with polynomial features compare to using only Linear regression and both regularizations alone.
2. In terms of accuracy and explainablity of the model, the Ridge Regression with polynomial features is the best for the main objectives of the analysis.


## Next Steps:
1. The dataset need more features for it to be a more better model, so there is need to add more relevant features to the dataset in the future.
2. Also, there is need to add more dataset in the future, because the more the data the better the model.


## Library Requirement:
For this project I used the following libraries:
1. [pandas](https://pandas.pydata.org/) For Data Manipulation and Data Analysis
2. [numpy](https://numpy.org/) For Scientific computation
3. [sklearn](https://scikit-learn.org/) For Machine Learing
4. [scipy](https://scipy.org/) For Mathematical computation
5. [seaborn](https://seaborn.pydata.org/) For Data Visualization
6. [matplotlib](https://matplotlib.org/) For Data Visualization


# Thanks for reading!!!