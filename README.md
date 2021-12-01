# Module_18_Cryptocurrencies
UNC Bootcamp - Module 18 - Classwork

## Overview 
This project was done to group and classify cryptocurrencies using unsupervised learning.  The dataset was from CryptoComare and was downloaded as a csv file.

## Deliverable 1: Preprocessing the Data for PCA
This had several parts to clean the data.  Only cryptocurrencies which were being traded, had no null values, and had values for mined coins were kept for processing.  The IsTrading column was dropped and the CoinNames were moved to a separate dataframe for later use.  The get_dummies() method was used to create variables for the Algorithm and ProofType and then the StandardScaler fit_transfrom function was used to standardize the features.

## Deliverable 2:  Reducing Data Dimensions Using PCA
The PCA algorithm was performed to reduce the data to three principal components and store the resulting dataset in a new dataframe.

## Deliverable 3: Clustering Cryptocurrencies Using K-means
An elbow curve was produced by using hvPlot to find the best K value.  The K-means algorithm was then run against the dataframe to make predictions on K clusters. Dataframes were combined and a new field was created to hold the predications.

## Deliverable 4: Visualizing Cryptocurrencies Results
A 3D scatter plot, using Plotly Express scatter_3d() function, was produced to show the three clusters from the previous dataframe.  A table of tradable cryptocurrencies was developed with the hvplot.table() function.  The MinMaxScaler().fit_transform method was used in creating the scatter plot.
