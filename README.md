# Back Propagation Alghoritm

Created: May 3, 2023 6:57 PM
Link: https://github.com/OsmanBuyuksar/NeuralNetwork
Tags: AI, Nureal Network, Python

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled.png)

### Summary

---

In this project i programmed a neural network from scratch using only numpy arrays. 

 - Coding process contains mathematical explanations and their code equivalents.

### Coding Process

---

The inner workings of the neural network consist of 2 mathematical steps which is:

1 - Forward Propagation

2 - Back Propagation

************Forward Propogation************

In forward propagation i need to calculate next layer values which can be calculated using this formula:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%201.png)

Since its a matrix multiplication operation i stored perceptron values in a vector and used  "`@`” for the forward propagation alghoritm and also squashed the values for it to give better results. Which results in this forward propagation function:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%202.png)

  

********************************Back Propagation********************************

For neural network to learn from its mistakes we need to calculate the error according to the weight parameters which can be obtained by using chain rule which is:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%203.png)

Because we are using sigmoid as squashing function gradient of  Perceptron value to its non-squashed value can be calculated with this formula:

![Untitled](Back%20Propagation%20Alghoritm%20f331bed106aa4d8c9d64ff008a5e9dc5/Untitled%204.png)

 Since there is no expected value for the hidden layers we are using next layers error to calculate hidden layers error which is 

### The design

---
