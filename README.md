# Multinomial-logistic-regression
This is a full design and implementation of multinomial  logistic regression to predict if a breast cancer patient should have chemotherapy before or after surgery or should go to multidisciplinary team . 
* Idea and objectives
* Implementation
* Output and evaluation
* Dataset
* Run

# Idea and objective
This model is made for an application that is dedicated to egyptian breast cancer patients of ABC center .
the classification problem has 3 ouputs YES , NO or MDT 

# Implementation
 - Linear model
 The linear model equation is the same as the linear equation in the linear regression model.
 for N features , the puput is as follows : y= w1x1 + w2x2 + ...+wn xn 
 
 - Softmax
 The Softmax function is a probabilistic function which calculates the probabilities for the given score. Using the softmax function return the high probability value for the high scores and fewer probabilities for the remaining scores . for every feature N
 - Cross entropy
 The Cross-entropy is a distance calculation function which takes the calculated probabilities from softmax function and the  one-hot-encoding matrix 
 
 - One hot encoding
 One-Hot Encoding is a method to represent the target values into a binary representation. For every feature the one-hot-encoding matrix is with the values of 0 and the 1 for the target class. The total number of values in the one-hot-encoding matrix is equal to the number of classes which is 3 in this dataset(yes\no\MDT)
 
 # Ouptut and evaluation
 Due to github non ability to render notebooks most of time , samples of output are screenshoted below .
 The accuracy of the training set and testing set is not around a stable range as the dataset isn't large and the training/testing split is random every run . One run is shown below
 
 ![alt text](https://github.com/yasminehatem/Multinomial-logistic-regression/blob/master/output%20images/training%20and%20testing%20sets%20accuracy.PNG)
 
 The prediction on the testing set is shown below using matplotlib
 
 ![alt text](https://github.com/yasminehatem/Multinomial-logistic-regression/blob/master/output%20images/testing%20set%20accuracy%20plot.png)
 
 To fix that I implemented a cross validation function to get the average accuracy and the results are shown below :
 
![alt text](https://github.com/yasminehatem/Multinomial-logistic-regression/blob/master/output%20images/training%20and%20testing%20sets%20accuracy.PNG)

# Dataset
This datset is auto generated  with respect to the medical standars . The students working on this data are cairo univeristy students:
1. Yasmine Hatem
2. Nermine Safwat
3. Ahmed Khalifa
4. Ahmed Khaled

The dataset is labeled and revised by M.D. Omar Sherif Omar

 # Run
 Dependencies
 - matplotlib.pyplot
 - Pandas
 - Numpy
 - sklearn.model_selection.train_test_split

