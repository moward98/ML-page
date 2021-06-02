This page is intended to show some of my past projects regarding Machine Learning.
## Project 1: Non-Linear Regression via Feedforward Neural Net w/ Back-propagation
The goal of this project was to create a neural net that could solve a non-linear regression equation. The neural net was created using keras, and scikit-learn was used for K-fold cross validation. During this project, I investigated the effect of varying the number of hidden nodes within the neural net, and the number of training data points the neural net was given.

The following is the non-linear equation that the model is trying to predict.

![](media/NLEqn.PNG)

The most accurate model created, was the one given the most amount of data points, and the most hidden nodes. It's prediction of the smooth curve is shown overlaid in red.

![](media/model.PNG)

## Project 2: Kohonen Self Organizing Map (KSOM)

Given an image comprised of random coloured pixels, I created a Kohonen Self Organizing Map to cluster similar hues into the same neighbourhoods. 

This is the initial image:

![](media/original.PNG)


Once I had created the KSOM, I studied the effects of changing the number of epochs run, as well as the initial neighbourhood radius (sigma). I learned that the more epochs ran, the smoother of a colour gradient was output, and that there was a fine line to having a neighbourhood radius not too large or too small. 
Some of the KSOM outputs studied are shown in the table below.


| Sigma = 10  | Sigma = 40|Sigma = 70|
| :-------------: |:---------------------------:|:-:|
|![](media/2010.PNG) |![](media/2040.PNG) |![](media/2070.PNG) |
|![](media/4010.PNG) |![](media/4040.PNG) |![](media/4070.PNG) |
|![](media/10010.PNG)|![](media/10040.PNG)|![](media/10070.PNG)|
|![](media/60010.PNG)|![](media/60040.PNG)|![](media/60070.PNG)|


## Project 3: MLP vs Deep Learning CNN Study
Using TensorFlow, Keras, and scikit-learn, I created a multi-layer perceptron and two deep learning CNN's  with different architectures to compare the training and testing accuracies of the models. I also evaluated the training times for each model. 

The model accuracies are:

![](media/accuracies.PNG)

These results indicate the CNN's are much more accurate than a multi-layer perceptron. CNN1 having a training accuracy so much higher than it's testing accuracy points towards the model being overfit. However, CNN2 having more balanced accuracies indicates it is the best model. 

The MLP accuracies over time are:

![](media/mlp.PNG)

The CNN1 accuracies over time are:

![](media/cnn1.PNG)


The CNN2 accuracies over time are:

![](media/cnn2.PNG)

The Model Training times are:

![](media/times.PNG)

