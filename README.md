# Neural_Network_Analysis

### Project Overview

The purpose of this project was to create a binary classifier with the ability to predict wether applicants should be granted funding from the company Alphabet Soup. The Neural Model is compiled after the data is processed and then the data is evaluated. It is attempted to optimize the model by increasing the accuracy to 75% or more. 

### Results

After analyzing the Dataframe of the "charity_data.csv" file, the "EIN" and "NAME" columns were dropped, since this information didn´t contain any valuable data that could be helpful for our analysis. 

Columns such as "APPLICATION_TYPE" and "CLASSIFICATION" which had more than 10 unique values, were binned into a new column ("Other"). A list of categorical variables was generated and encoded using "OneHotEnconder". The encoded data was added into a new DataFrame and the original data was dropped.

The variable "IS_SUCCSEFUL" was considered the target for this model, and all the other variables in the DataFrame were considered as features. 

In terms of the model, the Rectified Linear Unit (Relu) was used for the activiation of the function for the first and second hidden layers, and a
the Sigmoid activation function is used for the output layer. Also, a callback that saves the model weight every 5 epochs was set. After setting these parameters, the results that we had were the next:

![](https://github.com/JoseLuisMontemayor/Neural_Network_Charity_Analysis/blob/main/Resources/Test1.PNG)

We can see that the accuracy level was 72.88%, even though it´s a good percentage, it isn´t the score we were looking for. 

![](https://github.com/JoseLuisMontemayor/Neural_Network_Charity_Analysis/blob/main/Resources/Test2.PNG)

For the Optimization Model we just increased by 50 the application counts, which it didn´t make much of a difference, the accuracy actually decreased by .23%. Perhaps a real change in the result would be reflected by modifying the numbers of the hidden layers. 

### Summary 

With the trials conducted we weren´t able to produce a model with an efficiency level of at least 75%, even though we were close. There can be a variety of possibilites of why we didn´t reach our goal, the data that would need to be manipulated to approach the desired result would be the number of neurons in the hidden layers, the number of epochs per interval, and other outliers that could have been on the data.  
