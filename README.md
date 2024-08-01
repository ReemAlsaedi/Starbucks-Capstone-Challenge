# Starbucks-Capstone-Challenge
## Problem Statement:
The primary goal of the Starbucks Capstone Challenge is to analyze customer responses to various types of offers sent through the Starbucks rewards mobile app. Specifically, the project aims to:
1. Discover customer attributes and buying behavior based on the demographic and transactional data.
2. Predict how different demographic groups respond to various types of offers, including buy-one-get-one (BOGO), discount, and informational offers.
Using the provided data, I will examine which demographic groups are most responsive to each offer type and how spending behavior correlates with these offers. This analysis involves using classification supervised machine learning models to predict customer responses and evaluate the effectiveness of different offers.

## Dataset Overview:
The project utilizes three key datasets:
1. profile.json:
Contains information on 17,000 users of the rewards program with the following fields:
Rewards program users (17000 users x 5 fields)
- gender: (categorical) M, F, O, or null
- age: (numeric) missing value encoded as 118
- id: (string/hash)
- became_member_on: (date) format YYYYMMDD
- income: (numeric)

2. portfolio.json
Includes details about offers sent during a 30-day test period with the following fields:
- reward: (numeric) money awarded for the amount spent
- channels: (list) web, email, mobile, social
- difficulty: (numeric) money required to be spent to receive reward
- duration: (numeric) time for offer to be open, in days
- offer_type: (string) bogo, discount, informational
- id: (string/hash)
3. transcript.json
Contains event logs for 306,648 events with the following fields:
- person: (string/hash)
- event: (string) offer received, offer viewed, transaction, offer completed
- value: (dictionary) different values depending on event type
- offer id: (string/hash) not associated with any "transaction"
- amount: (numeric) money spent in "transaction"
- reward: (numeric) money gained from "offer completed"
- time: (numeric) hours after start of test

### Results
The analysis was conducted using various machine learning models to evaluate customer responses to different offers. The final model, a random forest classifier, achieved a training accuracy of 0.944 and an F1-score of 0.939. On the test data set, the model demonstrated an accuracy of 0.929 and an F1-score of 0.931, indicating that the model effectively generalized and did not overfit the training data. This model helps in understanding customer behaviors and optimizing marketing strategies for better engagement and higher conversion rates.


#### Blog post on Medium  
https://medium.com/@reemalsaedi6/starbucks-capstone-challenge-b5a91fcc997d

#### Install
This project requires Python 3.x and the following Python libraries installed:
- NumPy
- Pandas
- matplotlib
- scikit-learn
#### Udacity Data Scientist Nanodegree Capstone Project
This repository has all the code and report for my Udacity Data Scientist Nanodegree Capstone project.

#### Licensing, Authors, Acknowledgements, etc.
Data for coding project was provided by Udacity.
#### Blog post on Medium  
https://medium.com/@reemalsaedi6/starbucks-capstone-challenge-b5a91fcc997d
