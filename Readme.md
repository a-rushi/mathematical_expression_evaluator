# Handwritten Mathematical Expression Evaluator


## About
The model predicts the value of a mathematical expression given as an image by identifying individual components of the image.
We first divide the image into three segments at regular intervals and by using our prediction of whether the expression is in infix,prefix, or postfix
format we predict the digits and the operator in the image and manually calculate the value of the expression and compare it with the actual output. 

## Methods Used
 A] Train_Labels : Categorize the expression as infix, prefix,postfix
 B] Train_Oper : Identify the operator used
 C] Train_Dig : Identify the digit in the image

 Each of these models uses `convolutional neural networks` followed by `fully connected layers` with `3,4,10` output classes respectively.

 To train the model for classifying the expression as infix,prefix,postfix we have used the dataset already provided whereas to identify 
 the digits we have used the `MNIST` data set and to identify the operators we have used dataset available on `kaggle`.