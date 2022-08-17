# Neural_Network_Analysis

### Project Overview

The purpose of this project was to create a binary classifier with the ability to predict wether applicants should be granted funding from the company Alphabet Soup. The Neural Model is compiled after the data is processed and then the data is evaluated. It is attempted to optimize the model by increasing the accuracy to 75% or more. 

### Results

After analyzing the Dataframe of the "charity_data.csv" file, the "EIN" and "NAME" columns were dropped, since this information didn´t contain any valuable data that could be helpful for our analysis. 

Columns such as "APPLICATION_TYPE" and "CLASSIFICATION" which had more than 10 unique values, were binned into a new column ("Other"). A list of categorical variables was generated and encoded using "OneHotEnconder". The encoded data was added into a new DataFrame and the original data was dropped.

The variable "IS_SUCCSEFUL" was considered the target for this model, and all the other variables in the DataFrame were considered as features. 

In terms of the model, the Rectified Linear Unit (Relu) was used for the activiation of the function for the first and second hidden layers, and a
the Sigmoid activation function is used for the output layer. 
