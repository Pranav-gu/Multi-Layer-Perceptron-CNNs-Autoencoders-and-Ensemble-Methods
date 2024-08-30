# SMAI Assignment 3 and 4
# Name - Pranav Gupta
# Roll No. - 2021101095

# Asssignment 3

## Task 1 Logistic Regression ##
Everything is done according to the specifications of the Assignment and no big assumptions have been made regarding the task. Also the plots obtained have been attached in the Jupyter Notebook itself with their required explanations wherever asked.

## Task 2 MLPs for Classification ##
It is assumed while performing Hyperparameter Tuning in 2.2 and 2.3 that the number of neurons in each hidden layer remains the same. Also, wherever it is not mentioned which Activation Function or Optimiser is to be used, by default, Sigmoid and Batch-Gradient Descent are used. Cross Entropy Loss function is used for evaluating Loss.
In 2.4, although the number of neurons can vary in each hidden layer as well as done in the code. All metrics have been reported in the Assignment as specified.

## Task 3 MLPs for Regression ##
It is assumed while performing Hyperparameter Tuning in 3.2 and 3.3 that the number of neurons in each hidden layer remains the same. Also, wherever it is not mentioned which Activation Function or Optimiser is to be used, by default, Sigmoid and Batch-Gradient Descent are used. The metrics have been reported as asked in the assignment.

## Task 4 CNNs and Autoencoders ##
Data Visualisation and Preprocessing is done as is asked in the question. In 4.2, as asked in the question, suitable CNN Architecture has been developed to build the Model for Image Processing. 
In Hyperparameter Tuning 4.3, Tuning is done for only 2 architectures as specified in the Class itself. Also, the effect of Dropout has been considered in the sense that Dropout is Absent for the Model with the best performing set of Hyperparamaters and then it's accuracy is compared with the Model. Specifically, Kernel Sizes, Strides are not specifically varied but varied in the sense that the 2 architectures have different sizes of kernels, strides and paddings.
In 4.5 The Noisy Dataset is trained on the best performing Model and also, in 4.6, Autoencoders class is implemented in order to denoise the given noisy dataset. Correspondingly all metrics have been reported as mentioned in the assignment. 


# Asssignment 4
## Part 3 Ensemble Learning ##

### Part 3.1 Pre-Requisites ###
Classes for Logistic Regression, and MLPs have been taken from Assignment 3. So, Hyperparameters for the corresponding Classes have been taken from the Previous Assignment only. Only Linear Regression is implemented from Scratch and tuned over necessary Hyperparameters.

### Part 3.2 Bagging ###
Separate Functions for Bagging for Classification and Regression tasks have been written. The guidelines mentioned in the Assignment PDF have been followed and all necessary Hyperparameter Tuning has been done for the Bagging Methodology.
In Classification, Hard Voting is done by taking the Class having Maximum Probability for each data point and votes incremented for that particular class. It is repeated for all Models and correspondingly the Predictions of the Class with maximum Votes is picked. Soft Voting is done by first summing the Probabilties for Classes for all models and then the predictions of the Class having the max sum is picked.
In Regression, Hard Voting is done by taking the mean of predictions of all Models. Soft voting is done by first evaluating R2-Score on the Validation Set and then taking the weighted average of R2-Scores with the predictions.
Everything else has been done according to the Assignment.

### Part 3.3 Stacking ###
Separate Functions for Stacking for Classification and Regression tasks have been written. The guidelines mentioned in the Assignment PDF have been followed and all necessary Hyperparameter Tuning has been done for the Stacking Methodology.

## Part 4 Random Forest vs Boosted Trees ##
Random Forest, Adaboost Trees and Gradient Boosted Trees have been implemented from Scratch. Hyperparamter Tuning has been done and Accuracies and R2-Scores along with the Running Times of the Algorithms have been reported as specified in the Assignment. At the end, a brief theory has been provided for the results obtained and Part 4 3rd Point. 