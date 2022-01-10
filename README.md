# Neural_Network_Charity_Analysis

## Overview

The purpose of this project is to compare the difference between traditional machine learning and neural network models. We will be looking at the results and statistics from the two models summarize which method is better. 
Per given dataset we will be able to analyze which applicants are more likely to be succesfull in future. 

## Results

### Data Preprocessing

- What variable(s) are considered the target(s) for your model?
	- IS_SUCCESSFUL

- What variable(s) are considered to be the features for your model?
	- All except dropped and IS_SUCCESSFUL column

- What variable(s) are neither targets nor features, and should be removed from the input data?
	- EIN, NAME because these columns are non-beneficial


### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
For the regular ML model we chose 2 hidden layers and 1 output layer. However, in the optimization model I chose to go with 5 hidden layers and 1 Output layer.
With relu, sigmoid and linear function at the final layer. 

![](https://github.com/c3crocks/Neural_Network_Charity_Analysis/blob/main/Images/Method_Initial.JPG)

![](https://github.com/c3crocks/Neural_Network_Charity_Analysis/blob/main/Images/Method_Optimized.JPG)


- Were you able to achieve the target model performance?
The model was able to reach the target of almost 73%. 

![](https://github.com/c3crocks/Neural_Network_Charity_Analysis/blob/main/Images/accurace_Initial.JPG)

![](https://github.com/c3crocks/Neural_Network_Charity_Analysis/blob/main/Images/accurace_optimized.JPG)

- What steps did you take to try and increase model performance?
	- Dropping more unwanted columns such as STATUS, SPECIAL_CONSIDERATIONS and USE_CASE
	- Adding additional neurons and hidden layers in the model
	- Changing activation function 	


## Summary

The model got an accuracy of 73% after adding hidden layers and changing the later activation function from relu to combination of other functions. 
The model was overfitted in the first model since we saw a massive loss of accuracy to 46%. Also, removing some more unneccessary columns helped in the bump in accuracy. 