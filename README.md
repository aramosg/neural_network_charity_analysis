# Module 19 challenge - Neural Network charity analysis

## Overview of the analysis
We have been given a dataset showing the charitable organizations that have received funding from Alphabet. The purpose of this analysis is to use this dataset to create a classifier and determine if any given organization will be successful if funded by Alphabet.

## Results

### Data preprocessing
**What variable(s) are considered the target(s) for your model?**
The variable "IS_SUCCESSFUL" in the dataset is our target. After building our model we should be able to anticipate the values on this column.

**What variable(s) are considered to be the features for your model?**
The features are all other variables that are being used as inputs for the calculations. Columns such as "APPLICATION_TYPE", "CLASSIFICATION", "USE_CASE", and "INCOME_AMT" describe the organizations and were used to build the model.

**What variable(s) are neither targets nor features, and should be removed from the input data?**
Columns "EIN" and "NAME" are identification columns and do not add any value into the model. These columns were removed from the dataframe before building our model.

### Compiling, Training, and Evaluating the Model
**How many neurons, layers, and activation functions did you select for your neural network model, and why?**
The Neural Network was built with 2 hidden layers, each one with five nodes. "RELU" was selected as activation function. After some rounds of "trial and error", I noticed this combination was the one which provided the best performance.

**Were you able to achieve the target model performance?**
No. The highest accuracy achieved was 72%. 

**What steps did you take to try and increase model performance?**
Three different acitivites took place trying to improve the performance of the model:
1. Dropping "unnecesary" columns
2. Increasing the number of hidden layers and a different combination of nodes
3. Using different activation functions. 

### Summary
At the end, I was not able to improve the model's performance above 75%. Even though I tried different options, I could not get there. It may be worth it to consider different angles:

a. Do we have enough data? Perhaps, getting more descriptive data about the companies may be helpful to build a more robust model. 
b. Do we really need to build a Neural Network to solve this clasification problem? A simpler method may provide better results.

A simple classification model may be enough to achieve our goal. It really depends on the data we have and the precision we want to achieve. Sometimes, the simpler answer is the right one.