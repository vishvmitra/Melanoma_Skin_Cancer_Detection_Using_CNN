# Melanoma_Skin_Cancer_Detection_Using_CNN
> CNN based model which can accurately detect melanoma


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Conclusions
- We created a CNN Model using the image dataset (ISIC) with 3 convulated layers, 1 drop out layer(50%), 1 Flatten Layer,
  1 Dense Layer (relu) and 1 Output Layer with SoftMax activation function. We used Adam optimizer and categorical cross_entropy for loss function. 

- Without using the augmentor, the model did not perform well (Training Accuracy: 0.7048, Validation Accuracy: 0.5570). 
  This is because of underfitting. As there is a huge class imbalance wrt number of images for each class of data. 

- After using the augmentor, which helped to create additional images for classes with less data, it improved the model training
  significantly. The model performed really well on both training and Validation data set 
  (Training Accurary: 0.8247, Validation Accuracy: 0.7877)

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.*
- Pandas
- NumPy
- SeaBorn
- MatPlotLib
- SkLearn
- StatsModels
- TensorFlow
- Keras

## Acknowledgements
We implemented this project as part of the Advanced Regression Module required for Post Graduate Diploma in Machine Learning and AI - IIIT,Bangalore (April -2022 batch).
- This project was based on [this tutorial](https://learn.upgrad.com/course/2880).

## Contact
Created by Vishvmitra Belsare[@vishvmitra] - feel free to contact me!