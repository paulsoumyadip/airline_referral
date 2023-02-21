# airline_referral
# Airline_passenger_referal_prediction
Predicting aircraft passenger referal and excavating the main influencing factors can help airlines improve their services and gain. 

Airline_passenger_referal_prediction

![readme photo](https://user-images.githubusercontent.com/109894515/203723816-18bffc0e-eb59-4a38-9fbf-b4e5740734c0.jpg)

Air transport or aviation plays a very important role in the present transport structure of the world and surely it is considered the gift of the twentieth century to the world. In today’s fast-paced world, air transport has been a blessing to all because of its speed of transportation. This mode of transport is very useful to get the products with short delivery times quickly and safely to those who require it also allows the tourism industry in each country to have stable growth by shortening the distance among all the people who inhabit the world. Here, I have a dataset regarding the ratings of services provided by different airlines to customers. The main objective of this project is to understand how likely the passengers will recommend the airlines to others. The dataset here is quite large which initially had 131895 rows and 17 columns. On checking the data information, it was derived that there were basically two different types of data in the dataset there are 7 columns of floats64, data types 10 columns with object types. Coming to the null values and missing values in the dataset, it was observed that there was a mismatch in the non-null counts which clearly stated that a large number of missing and null values were present in the dataset.

Data is scrapped in the Spring of 2019 from the Skytrax website. Data includes airline reviews from 2006 to 2019 for popular airlines around the world with multiple-choice and free-text questions. The main objective is to predict whether passengers will refer the airline to them or not.


<p><b>Objective</b>: The main objective is to predict whether passengers will refer the airline to their friends.</p>

<p><b>Description of features in the dataset</b>:
  <li>airline: Name of the airline.</li>
  <li>overall: Overall point is given to the trip between 1 to 10.</li>
   <li>author: Author of the trip</li>
   <li>review date: Date of the Review customer review: Review of the customers in free text format</li>
   <li>aircraft: Type of the aircraft</li>
   <li>traveller type: Type of traveler (e.g. business, leisure)</li>
   <li>cabin: Cabin at the flight date flown: Flight date</li>
  <li>seat comfort: Rated between 1-5</li>
   <li>cabin service: Rated between 1-5</li>
   <li>foodbev: Rated between 1-5 entertainment: Rated between 1-5</li>
   <li>groundservice: Rated between 1-5</li></p>
   
  <p><b>Data Preparation</b>:
   <li> Dropping rows having entire row as NAN</li>
   <li>Dropping columns which don't add value for the analysis</li>
  <li>Dropping duplicates</li></p>
  
<p><b>EDA</b>:
 The primary goal of EDA is to support the analysis of data prior to making any conclusions. It may aid in the detection of apparent errors, as well as a deeper understanding of data patterns, the detection of outliers or anomalous events, and the discovery of interesting relationships between variables.</p>
  
  
<p><b>Feature Engineering</b>:
  Engineered new features based on-
  <li>Date of travel</li>
  <li> review text such as polarity using VADER.</li>
  <li>overall rating column such as positive or negative review</li>
  <li>onehot encoding on cabin_type ,Airlines and travller_type to create new features.</li>
</p>

<p><b>Model Building</b>:
  Built different classifier models such as
  <li>Logistic Regression</li>
  <li>DecisionTree</li>
  <li>XG Boost</li>
  <li>SVM</li>
  <li>Random Forest</li>
  <li>K-Nearest Neighbour</li>
  

  
 <strenght>The performance is exceptionally good but we saw a scope of improvement where we can detect anomalies and replace the recommended column with the correct one.
All models are working great on this dataset and getting a good range of accuracies around 95%, which is pretty good. But to make sure our model is not in an overfitting condition performing cross validation techniques would help.GridSearchCV and Cross Validation techniques used are K-fold and Repeated K-fold. At every fold accuracy is 95% only this means that the models are actually working well on models.</strenght>
</p>
<p>
