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
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Not all users receive the same offer, and that is the challenge to solve with this data set.

Your task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

Every offer has a validity period before the offer expires. As an example, a BOGO offer might be valid for only 5 days. You'll see in the data set that informational offers have a validity period even though these ads are merely providing information about a product; for example, if an informational offer has 7 days of validity, you can assume the customer is feeling the influence of the offer for 7 days after receiving the advertisement.

You'll be given transactional data showing user purchases made on the app including the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record for each offer that a user receives as well as a record for when a user actually views the offer. There are also records for when a user completes an offer.

Introduction
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Not all users receive the same offer, and that is the challenge to solve with this data set.

Your task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

Every offer has a validity period before the offer expires. As an example, a BOGO offer might be valid for only 5 days. You'll see in the data set that informational offers have a validity period even though these ads are merely providing information about a product; for example, if an informational offer has 7 days of validity, you can assume the customer is feeling the influence of the offer for 7 days after receiving the advertisement.

You'll be given transactional data showing user purchases made on the app including the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record for each offer that a user receives as well as a record for when a user actually views the offer. There are also records for when a user completes an offer.

Keep in mind as well that someone using the app might make a purchase through the app without having received an offer or seen an offer.

## Results
---> We built an ML model that predicts whether the customer prefers and would select BOGO or Discount. From the results above, we can see that system classifies the customer by giving prediction about how would they respond to the offer. If we get Prediction for both BOGO and Discount as 1, then the customer uses both. If we get 0 for both which means that we don't need to send the customer offers.

--> The model above predicts the results on the basis of age, gender, income and the year and month when the cutsomer joined.

--> We compared two ML models for the analysis, i.e. KNClassifier and ADABoostClassifier. ADABoostClassifier gave us better results and thus was chosen.


Please find the blog for the project here:
https://starbuckscapstone.blogspot.com/2020/06/starbucks-capstone-challenge.html
