# cmps144_project
repository for cmps 144 (applied ml) group project

contributors: Cody, Paulo, Cameron

# Predicting Kickstarter Project Outcomes
This repository contains a Kickstarter dataset and jupyter notebooks for predicting  
whether a given Kickstarter project will meet its funding goal.   

* kickstarter_project.ipynb contains all of our data vissualization as well as a deep  
neural network.

* cleaned_144_project.ipynp only contains cells necessary for the deep neural net.

* Project architecture:  
We began by converting some of the string-based columns to numerical columns and  
simplifying our project states. Instead of dealing with four project states we  
decided to simply use binary states for success and failure. We then generated  
various additional features such as duration of projects and success rate for  
project categories. Once our features were created, we scaled numerical features  
and created one-hot-encodings for string features. The dataset was then split into  
train/validation and test data. This data was then fed into a deep neural network  
with four hidden layers. Each layer, except the output, has the ReLU activation  
function with 40-50% dropout. We then trained the model using mean-squared-error  
and or binary-categorical-cross-entropy for 50 epochs. 
