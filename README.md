# CNN model for Melanoma Cancer detection
> This is a project to build a CNN model to detect Melanoma cancer.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Outcome of Model Development](#Outcome-of-model-development)
* [Recommendations](#Recommendations)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Introduction
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. Its of atmost importance to detect the presence of these cells beforehand so that chances of it being fatal can be drastically brought down.

### Problem Statement
Since Melanoma is malignant, its of utmost importance to detect the presence of these cells at the earlist. We need to build a CNN based model which can accurately detect melanoma.  A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis

### About the Dataset
We are provided with close to ***2239*** images of around 9 different cancerous patches on the skin. These images are of the size 180*180 pixels. 


## Technologies Used
- numpy - 1.16.2
- pandas - 0.24.2
- matplotlib - 3.0.3
- seaborn - 0.11.2
- statsmodels - 0.9.0
- scikit-learn - 0.20.3
- tensorflow - 2.8.0

## Outcome of Model Development
We initially started off with building couple of models: one without the dropout layer and one with the dropout layer. In both the case, we found that the accuracy of training dataset was around 45% and valdiation accuracy was around 50%. The accuracy was very less, ans also the fact that validation accuracy was lesser than the training accuracy suggested that there was underfitting.

Upon observation, we found that there was a serious class-imbalance. One way of resolving this issues was the use of Data augmentation technique. Using the data augmentation technique, we were able to add 500 samples for each of the class and hence were able to reduce the affects of class-imbalance. After building the model on top of this new dataset, we ***acheived training accuracy of 72% and validation accuracy of 69%***. With this, we improved our model performance by 50% as compared to previous attempt and also mitigated the probelm of over-fitting and under-fitting. 

## Contact
Created by [@RohanShetty12] - feel free to contact me!
