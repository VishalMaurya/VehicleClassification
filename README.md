# VehicleClassification

## Data Description:  
The data contains features extracted from the silhouette of vehicles in different angles. Four "Corgie" model vehicles were used for the experiment: a double decker bus, Cheverolet van, Saab 9000 and an Opel Manta 400 cars. This particular combination of vehicles was chosen with the expectation that the bus, van and either one of the cars would be readily distinguishable, but it would be more difficult to distinguish between the cars. 

## Context: 
The purpose is to classify a given silhouette as one of three types of vehicle, using a set of features extracted from the silhouette. The vehicle may be viewed from one of many different angles. 

## Attribute Information:
All the features are geometric features extracted from the silhouette.  
All are numeric in nature.

## Objective:  
Apply dimensionality reduction technique – PCA and train a model using principal components instead of training the model using raw data. 

Useing Support vector machines to classify the class(y) of vehicles and find the difference of accuracy with and without PCA on predictors(X). 
Using grid search (try C values - 0.01, 0.05, 0.5, 1 and kernel = linear, rbf) and find out the best hyper parameters and do cross validation to find the accuracy.

## Conclusoin:
We have achived 0.98, 0.98 0.96 score in f1-score column for bus, car, and van respectively.

Best parameters:
svc_param = {'C': 100, 'gamma': 0.1, 'kernel': 'rbf'}
pca_param = {'n_components':9}
Best score on Test data: 97.951 %
