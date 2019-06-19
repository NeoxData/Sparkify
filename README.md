# Sparkify
Udacity capstone project for Data science nanodegree

## Purpose
This project is to use the Apache Spark framework (Spark MLlib) on an AWS cluster for training a machine learning model with a large dataset (12GB).

The aim is to predict the churn rates of users from a digital music service Sparkify. There are subscription and free plan. The project is to create a model which can predict which user is about to leave the service. Some action can be taken then to keep him/her with discount for example.

## Installation
-  Python 3.5
-  PySpark ML
-  Jupyter
-  AWS EMR : registration to be made on the website of Amazon

## File description

Sparkify.ipynb : This is the initial notebook used for training and analysis. The dataset has a size of 128 MB. 

Sparkify_AWS.ipynb : this notebook uses the entire dataset (12GB).

Readme : explanation of project and tools used

## Feature and model

I have used a Logistic Regression model tuned the regularization parameter, using 3-fold cross validation. I splitted dataset in training and testing set (80-20).
The features used ("userAgent", "gender", "page","level","Churn") were engineering with a stringIndexer.

## Blog Post Link
https://medium.com/@neoxData/how-to-predict-customer-churn-on-huge-dataset-cd36ea15e3ac

## References
Dataset provided by Udacity (s3n://udacity-dsnd/sparkify/sparkify_event_data.json)

Official pySpark documentation has also been used "https://spark.apache.org/docs/latest/api/python/index.html"
