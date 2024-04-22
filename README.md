# Back Propagation Alghoritm

Tags: AI, Nureal Network, Python

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled.png)

## Summary

---

In this project a neural network consisting of several hidden layers are programmed from scratch using only numpy arrays for learning purposes. 

 - Below paragraphs detail the logic begind the programmed neural network.

## Coding Process

---

The inner workings of the neural network consist of 2 mathematical steps which is:

1 - Forward Propagation

2 - Back Propagation

************Forward Propogation************

In forward propagation we need to calculate next layer values which can be calculated using this formula:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%201.png)

Since we need to do a matrix multiplication operation perceptron values are stored in a vector. That way perceptron values can be multiplied seamleasly by using "`@`” symbol. After the matrix multiplication calculated values are squashed and stored. The way matrix multiplication performed is shown below:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%202.png)

  

********************************Back Propagation********************************

For neural network to learn from its mistakes we need to calculate the error according to the weight parameters which can be obtained by using chain rule which is shown below:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%203.png)

Because we are using sigmoid as squashing function gradient of Perceptron value to its non-squashed value can be calculated with this formula:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%204.png)

 Since there is no expected value for the hidden layers we are using the next layer error to calculate hidden layer error. That formula can be seen below: 

!![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%205.png)

 After calculating the error for each perceptrons chain rule can be applied to each of them to calculate the change in weights for the output. Then the change in weights are multiplied with the learning factor and final value is subtracted from the actual weights to update the weights. The code segment that is calculating the back propagation is shown below: 

 ![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%206.png)


## Prediction

 For training the network forward and backward propogations are performed sequentially for each data. After the training set is done, prediction of the model for any given test set is calculated by using forward propagation on the given data. 

---
