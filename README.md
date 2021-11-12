# Project 4: Team Hackathon

Pick a Kaggle competition from the following list. You have the choice of completing a regression problem, a classification problem, or an NLP problem involving either classification or sentiment analysis.

## Selected Topic
We chose to present on intel image classification per Kaggle competition below.
 [Intel Image Classification](https://www.kaggle.com/puneet6060/intel-image-classification)

## Exploratory Data Analysis

We read in image files and found that not all were the stated 150x150.  We wrote a function to resize any missized images before storing in a list that we converted to a numpy array of shape (150,150,3).

We processed the target data using a dictionary to convert names to numeric values corresponding to the Kaggle competition values.  

## Modeling

We implemented a neural network using two convolution layers, two pooling layers and three dense layers in addition to the input and output.  

Sequential model

Convolution,  (3,3), 8 filters
Pooling layer, (3,3)

Convolution,  (9,9), 16 filters
Pooling layer, (9,9)

Dense layer 300
Dense layer 150
Dense layer 25

Output layer 6


We tested the convolution sizes, the number of dense layers and the number of filters.  We also tested regularization with Dropout but our best model so far did not implement Dropout.  

## Metrics

The model training accuracy of 0.79 and a testing accuracy of 0.77.  

## Conclusions and Next steps

We built a neural network model that showed reasonable performance on the training and testing set.  Given more time we would look at regularization and training longer (more CPU power).  
