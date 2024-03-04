## Neural Network Model Report

# Overview

The purpose of this neural network model was to help the nonprofit foundation Alphabet Soup choose the most suceesful candiates for funding. 

# Data Preprocessing
        
* The variable for the target is the coloumn:

  IS_SUCCESSFUL

* The variables for the features are the coloumns:

   NAME
   APPLICATION_TYPE
   AFFILIATION
   CLASSIFICATION
   USE_CASE
   ORGANIZATION
   STATUS
   INCOME_AMT
   SPECIAL_CONSIDERATIONS
   ASK_AMT
   
* The variable that can be removed from the data is the coloumn:

   EIN

# Compiling, Training, and Evaluating the Model

I used 3 hidden layers in both the original and optimsed model. they were tanh and 2 sigmoid layers with the same number of neurons in both models. In the original model the accuray score came out as 72% however with optimisations I was 
able to increase that to 79%.

To increase the accuray of the model I made a couple of changes. First instead of dropping the 'NAME' coloumn I kept it but limited it to names that only appeared more than 5 times. Secondly I increased the cuttoff value for application types and 
classification types to 1000 from 500 and 100 respectively. 

Making just these two simple changes was enough to increase the accuray from 72% to 79%.

# Summary 

Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

Overall with optimisation we are able to correctly classify the test data 79% of the time if the applicant appears more than 5 times in the data. I think maybe using a different model such as PyTorch would be interesting to see the results 
as it's amore flexible and intuitive model.
  
