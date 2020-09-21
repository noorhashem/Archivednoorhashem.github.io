---
layout: post
title:  "Deeplearning.ai Neural Networks and Deep Learning Week 1 & Week 2"
categories: [ Machine Learning ]
image: 
author : Noor
---




# Week 1






# Week 2

## Logistic Regression as a Nerual Network

Logistic regression is an algorithim for binary classification.
A binary classification problem that a neural network could solve is a cat calssifier that tells from an image wether there is a cat present or not, to handle images for binary classification, it should be converted into feature vectors.

i.e) an image of 64px is converted into a feature vector of 64X64X3 size = 12288 (n), since its RGB values are going to be matrices of 64X64 size.

### Notation

<img src="/assets/images/PostsImages/DeepLearningCoursera1Blog1/Screen Shot 2020-09-21 at 3.23.44 AM.png" alt="notation shot" width="700">


 * Training example -> (x,y), where x belongs to the feature vector of size n and y belongs to the output vector of values of either {0,1}.

 * m -> training examples set : {(x^(1),y^(1)),(x^(2),y^(2).....)}

 * X -> feature matrix, where each column is a single training example's feature vector values X^(1), X^(2), X^(3), and each row is a single feature's values across the different training examples. so the feature matrix size = m (# of training examples) x nx (number of features in each feature vector)

 * Y -> output matrix, is a matrix of size 1xm, it's basically a matrix of one row and multiple columns that constitutes the outputs per training example y^(1),y^(2),y^(3)...y^(m)


### Logistic Regression

<img src="/assets/images/PostsImages/DeepLearningCoursera1Blog1/Screen Shot 2020-09-21 at 2.34.11 AM.png" alt="notation shot" width="700">

In logistic regression we take an input which is x that belongs to a feature vector of size nx and we want to output a value either 0 or 1, this can be an indication of the probability of the occurance of a certain event (a photo that has a cat in it), given a certain x as an input y^ = P(y=1 | x)

and with having w and b as parameters to these inputs that can affect this probability or y^, the output must be dependant on w and b. but multiplying the transpose of w with X and adding b vector will yield numbers that can be bigger than 1 or smaller than 0, so to limit the output to these two duels we insert our equation into a sigmoid function that evaluates the output into either a 0 or a 1 depending on w and b in our equation which now we call it Z as an input to the sigmoid function.







