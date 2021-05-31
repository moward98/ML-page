## Project 1: Non-Linear Regression via Feedforward Neural Net w/ Back-propagation
The goal of this project was to create a neural net that could solve a non-linear regression equation. The neural net was created using keras, and scikit-learn was used for K-fold cross validation. During this project, I investigated the effect of varying the number of hidden nodes within the neural net, and the number of training data points the neural net was given.

The following image is the original non-linear equation the model is trying to predict. 
![](media/NLEqn.PNG)

The most accurate model created, was the one given the most amount of data points, and the most hidden nodes. It's prediction of the smooth curve is shown overlaid in red.

![](media/model.PNG)

## Project 2: Kohonen Self Organizing Map (KSOM)

Given an image comprised of random coloured pixels, I created a Kohonen Self Organizing Map to cluster similar hues into the same neighbourhoods. 
<p align="center">
  <b>Initial Random Image</b><br>
  <img src="https://github.com/moward98/ML-page/blob/main/media/original.PNG">
</p>



Once I had created the KSOM, I studied the effects of changing the number of epochs run, as well as the neighbourhood radius. I learned that the more epochs ran, the smoother of a colour gradient was output, and that there was a fine line to having a neighbourhood radius not too large or too small. 
Some of the KSOM outputs studied are shown in the table below.


| Sigma = 10  | Sigma = 40|Sigma = 70|
| :-------------: |:---------------------------:|:-:|
|![](media/2010.PNG) |![](media/2040.PNG) |![](media/2070.PNG) |
|![](media/4010.PNG) |![](media/4040.PNG) |![](media/4070.PNG) |
|![](media/10010.PNG)|![](media/10040.PNG)|![](media/10070.PNG)|
|![](media/60010.PNG)|![](media/60040.PNG)|![](media/60070.PNG)|


The colour density of the points represents the probability that the space is occupied (darker = higher probability).

## Project 4: Fuzzy Logic Control of Inverted Pendulum
Given a set of fuzzy rules and the system illustrated below, this project involved creating membership diagrams of said rules, and then using the to create a fuzzy inference for a given system state. 

![](media/system.PNG)

The four membership rules are shown below. The state of the vertical angle and the angular velocity of the pendulum, determine the current of the DC Motor required to keep the pendulum upright.

![](media/membership.PNG)

Given a system state where the angle is 5° and the angular velocity is 15°/sec, the following fuzzy inference can be obtained.





