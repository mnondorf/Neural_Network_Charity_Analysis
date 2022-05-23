# Neural_Network_Charity_Analysis

## Overview
The purpose of this project was to use Neural Networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by the client, Alphabet Soup.

# Results

    Data Preprocessing:
    - What variable(s) are considered the target(s) for your model?
        - The target variable is 'IS_SUCCESSFUL', which tracks whether or not the money was used effectively. 
    - What variable(s) are considered to be the features for your model?
         - The features are: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', and
 'INCOME_AMT'.
    - What variable(s) are neither targets nor features, and should be removed from the input data?
        - 'EIN' and 'NAME'

    Compiling, Training, and Evaluating the Model:
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
        - We initially used a total of 16 neurons, 2 layers, and 2 activation functions.
        - For the optimization attempt, we removed an additional unnecesarry column ('SPECIAL_CONSIDERATIONS'), increased the number of neurons in the two original layers to 50 and 10, and added a third hidden layer with 5 neurons. We also tried out a tanh activation feature to see if it helped our results. 
        

    - Were you able to achieve the target model performance?
        - No, our best performance when "optimizing" only achieved ?% accuracy

    - What steps did you take to try and increase model performance?
        - We adjusted the number of neurons both up and down, added a 3rd hidden layer, and tried various combinations of activation functions.


# Summary 


Overall, the neural network model results were disappointing. The inital model only reached 72.8% accuracy with 55% loss and the "optmized" model barely nudged upward to 74% with 53% loss. It is possible that the model is overfitted. Perhaps using fewer epochs could improve training. 

A Random Forest model might be a better fit for this situation because it deals with categorical variables better.