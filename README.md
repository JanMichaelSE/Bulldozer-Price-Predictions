# Bulldozer-Price-Predictions


## Predicting the Sale Price of Bulldozers using Machine Learning

In this notebook, we're going to go through an example machine learning project with the goal of predicting the sale price of bulldozers.


## 1. Problem Definition

> How well can we predict the future sales price of a bulldozer, given its characteristics and prevoius examples of how much similar bulldozers have been sold for?

## 2. Data

The data is download from the Kaggle Blue Book for Bulldozers competition:

* https://www.kaggle.com/c/bluebook-for-bulldozers/data

There are 3 main datasets:

* Train.csv is the training set, which contains data through the end of 2011.
* Valid.csv is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
* Test.csv is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012. Your score on the test set determines your final rank for the competition.

## 3. Evaluation

The evaluation metric for this competition is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

For more on the evaluation of this project check:
* https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation

Note: The goal for most regression evaluation metrics is to minimize the error. So we'll minimize the RMSLE.
## 4. Features

Kaggle provides a data dictionary detailling all of the features of the datasets:
* https://www.kaggle.com/c/bluebook-for-bulldozers/data

## 5. Modelling

Started by diving into Random Forest Regressor as a first option (Still experimenting). Found some great results out of model so far by managing to achive a RMSLE score of 0.24524163989538328. This managed to rank in top top 30. Also included other metrics into account to have a better understanding of the results like: MeanAbsolutError and R^2 score

At the end we took a look at our **Feature Importance** to see what values could be more important to catch in the future to have a better model.

## 6. Experimentation
Repeat the procces the find areas of improvement.

Note: Will try to do a RandomizedSearchCV with more iterations to find better paramters but taking into account the amount of time it might take to complete the Search.
