# Starbucks_Capstone_Challenge <br>

## Libraries Used
pandas <br>
numpy <br>
math<br>
json<br>
matplotlib.pyplot <br>
seaborn <br>
datetime <br>
time <br>
warnings<br>
warnings.filterwarnings("ignore")<br>
sns.set_palette("pastel")<br>
sklearn.model_selection <br>
sklearn.ensemble <br>
sklearn.metrics <br>
sklearn.neighbors<br>
% matplotlib inline<br>

## Motivation
This is the capstone project to complete udacity Data Scientist Nanodegree. I've chosen Starbucks data that mimics customer behavior on the Starbucks rewards mobile app, and build a model to predict the preferred offer by the clients. <br>

## Introduction

The dataset contains simulated data from the Starbucks rewards mobile app that mimics the customer behavior. Starbucks sends out offers to the users every few days. These are generally categorized in to BOGO, discount or advertisements. 

In this project, I have used the data sets provided by starbucks and combined them to get the desired dataframe, on which I apply various ML models. The puporse is to come up with a classifier that predicts which offer would the customer most likely use. 

I have used the libraries mentioned above and tried to present few insights by vizualizing the data as well as predicting the customer behavior. The data that I have used consists of three data sets in which we get customer profiles, offer descriptions and transaction history.

## Results
--> I built an ML model that predicts whether the customer prefers and would select BOGO or Discount. From the results above, we can see that system classifies the customer by giving prediction about how would they respond to the offer. If we get Prediction for both BOGO and Discount as 1, then the customer uses both. If we get 0 for both which means that we don't need to send the customer offers.

--> The model above predicts the results on the basis of age, gender, income and the year and month when the cutsomer joined.

--> I compared two ML models for the analysis, i.e. KNClassifier and ADABoostClassifier. ADABoostClassifier gave us better results and thus was chosen.

--> For the purpose of validation, I used two approaches:

Comparing Models: I compared the accuracy of the KNeighbor Classifier with ADABoostClassifier and for this, I used precision, recall and f-1 score. The values were close by and the results were as expected. KNeighborClassifier is expected to perform poorly than the ADABoostClassifier and thus it was good enough to say that the model was satifactory. Even though the KNeighbors fit the data well, it performed poorly in prediction. Thus, it was tending to overfit.
Using test data to validate results: The original data was split into train and test data set and the model was trained on the trained data set. The trained model was then used to predict the target variables from the test dependent variables. Once the predicted target variables were received, I compared them with the actual target variables from the test data set to get the difference. The f-1 score for this was around 66% and thus, the model was validated. f-1 score was considered becasue it takes into consideration, both the precision as well as recall of the model.
--> Initially, I was just using the percentage of the times the customer has used an offer and was trying to predict that. I expected my output to be in a form of percentage. But I didn't get expected results. So I assigned the target variable the value 1 if it this percentage was greater than 75% and 0 if not. And thus, my target variable was a boolean. This helped me in getting the results.


Please find the blog for the project here:
https://starbuckscapstone.blogspot.com/2020/06/starbucks-capstone-challenge.html
