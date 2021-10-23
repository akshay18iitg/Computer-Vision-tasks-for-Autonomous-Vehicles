# Computer-Vision-tasks-for-Autonomous-Vehicles

This repository is part of work done during the competition of AI Blitz XI held by Blitz XI on AIcrowd platform.

![image](https://user-images.githubusercontent.com/50731752/138456397-bbddbeab-3111-4c9e-bb09-0634436dcaa0.png)

The competiton consists of 5 different problem statements related to autonomous vehicles.We tried to implement innovative ideas for this problem statements and secured overall rank of 9th.

## 1. Obstacle Prediction

In this **Classification problem statement**,radar sensor points where collected by mounting radar on self driving vehicle and running it in Carla Simulator.

![image](https://user-images.githubusercontent.com/50731752/138458976-2ed235c1-b1e5-4fc4-ac69-2503df390552.png)

- I collected some data in addition to given data to increase the dataset.Also used **SVM-Smote techniques** as dataset was imbalanced. 
- I tried various machine learning algorithm for classification, but achieved good accuracy by using **lightgbm algorithm**. 
- To further increase the f1-score, hyperparameter optimization was carried out by using **Bayesian Optimazation**. 
- To avoid overfitting, ensembling models is the best way. I ensembled 3 models by training them on 3 different dataset, created by cross validation, and achieved     **f1-score of 0.908**.


## 2. Lidar Car Detection

In this **Regression problem statement**,3D car lidar features from the dataset should be used to build an automated algorithm to predict how many vehicles were there in the lidar range.

![image](https://user-images.githubusercontent.com/50731752/138460449-d1e23ec4-feff-4c10-bba8-1ea126ad462a.png)

- I tried various machine learning algorithm for regression, but achieved good accuracy by using **xgboost algorithm**. 
- To further reduce loss, hyperparameter optimization was carried out by using **Bayesian Optimazation**. 
- It achieved  **mean error of 14.000** on private leaderboard. Would have been better if i had reduced overfitting.


## 3. Environment Classification

In this **Image Clustering problem statement**,we have to classify the weather into 5 different categories without any labels.

![image](https://user-images.githubusercontent.com/50731752/138540918-46cb0044-3645-4b37-ac1c-946fb13e3222.png)

- I tried various pre-trained imagenet models for **feature extraction**, but achieved good accuracy by using **Resnet architecture**. 
- For clustering i tried various clustering techniques, but achieved good accuracy by using **Guassian Mixture Model**.
- To avoid overfitting, ensembling models is the best way. I ensembled 3 models by training them on 3 different dataset, created by cross validation, and achieved     **score of 0.621**.


## 4. Object Detection

In this **Object Detection problem statement**,given dataset contains the images and the labels in MS COCO json format and over 4 classes, bicycle, motorcycle, passenger car, and person.


![image](https://user-images.githubusercontent.com/50731752/138541220-26ff6bbc-0f9a-463a-8366-9cca6fb161ba.png)

