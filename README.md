## Project 1: Non-Linear Regression via Feedforward Neural Net w/ Back-propagation
The goal of this project was to create a neural net that could solve a non-linear regression equation. The neural net was created using keras, and scikit-learn was used for K-fold cross validation. During this project, I investigated the effect of varying the number of hidden nodes within the neural net, and the number of training data points the neural net was given.

The following image is the original non-linear equation the model is trying to predict. 
![](media/NLEqn.PNG)

The most accurate model created, was the one given the most amount of data points, and the most hidden nodes. It's prediction of the smooth curve is shown overlaid in red.

![](media/model.PNG)

## Project 2: Kohonen Self Organizing Map (KSOM)

random coloured pixels. 
cluster colours of similar shade into the same neighbourhood.
Study effects of neighbourhood radius, and number of epochs run
Want neighbourhood radius not too large or too small, higher epochs the better. 
Look at the outputs.

| Original Image  | Semantic Segmentation Output|
| :-------------: |:---------------------------:|
| ![](media/Image1.PNG) | ![](media/SegImg1.PNG)|
| ![](media/Image2.PNG) | ![](media/SegImg2.PNG)|
| ![](media/Image3.PNG) | ![](media/SegImg3.PNG)|

The colour density of the points represents the probability that the space is occupied (darker = higher probability).

## Project 4: Fuzzy Logic Control of Inverted Pendulum
Given a set of fuzzy rules and the system illustrated below, this project involved creating membership diagrams of said rules, and then using the to create a fuzzy inference for a given system state. 

![](media/system.PNG)

The four membership rules are shown below. The state of the vertical angle and the angular velocity of the pendulum, determine the current of the DC Motor required to keep the pendulum upright.

![](media/membership.PNG)

Given a system state where the angle is 5° and the angular velocity is 15°/sec, the following fuzzy inference can be obtained.





