# Distracted Driver Detection

## Project Overview

According to the CDC motor vehicle safety division, one in five car
accidents is caused by a distracted driver. Sadly, this translates to 425,000
people injured and 3,000 people killed by distracted driving every year.

In this project, I have created and refined machine learning models to detect
what the driver is doing in a car given driver images. This is done by
predicting the likelihood of what the driver is doing in each picture. 

## Problem Statement

Given a dataset of 2D dashboard camera images, an algorithm needs to be
developed  to classify each driver's behaviour and determine if they are
driving attentively, wearing their seatbelt, or taking a selfie with their friends in
the backseat etc..? This can then be used to automatically detect drivers
engaging in distracted behaviours from dashboard cameras.

Following are needed tasks for the development of the algorithm:

1. Download and preprocess the driver images

2. Build and train the model to classify the driver images

3. Test the model and further improve the model using different techniques.

## Data Exploration

The provided data set has driver images, each taken in a car with a driver
doing something in the car (texting, eating, talking on the phone, makeup,
reaching behind, etc). This dataset is obtained from Kaggle(State Farm
Distracted Driver Detection competition).Following are the file descriptions and URL’s from which the data can be
obtained :
* imgs.zip - zipped folder of all (train/test) images
* sample_submission.csv - a sample submission file in the correct format
* driver_imgs_list.csv - a list of training images, their subject (driver) id, and
* [class id](https://www.kaggle.com/c/state-farm-distracted-driver-detection/download/)
* [driver_imgs_list.csv.zip](https://www.kaggle.com/c/state-farm-distracted-driver-detection/download/)
* [sample_submission.csv.zip](https://www.kaggle.com/c/state-farm-distracted-driver-detection/download/)

The 10 classes to predict are:

* c0: safe driving

* c1: texting - right

* c2: talking on the phone - right

* c3: texting - left

* c4: talking on the phone - left

* c5: operating the radio

* c6: drinking

* c7: reaching behind

* c8: hair and makeup

* c9: talking to passenger

There are 102150 total images. Of these 17939 are training images,4485
are validation images and 79726 are training images. All the training,
validation images belong to the 10 categories shown above.

