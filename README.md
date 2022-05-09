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
        - 'EIN', 'NAME', and 'SPECIAL_CONSIDERATIONS'

    Compiling, Training, and Evaluating the Model:
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
        - We used a total of 16 neurons, 2 layers, and 2 activation functions. We chose 8 neurons because best practice says to use 2-3 times the number of inputs for your neuron count. We chose 2 hidden layers because we testing including a third and it produced no added value. We chose 2 activation features (relu and sigmoid) both because they are the most common and because other combinations returned similar or worse results. 

    - Were you able to achieve the target model performance?
        - No, our best performance when "optimizing" only achieved 65% accuracy

    - What steps did you take to try and increase model performance?
        - We adjusted the number of neurons both up and down, added a 3rd hidden layer, and tried various combinations of activation functions.


# Summary

Overall, the neural network model results were disappointing. The inital model only reached 63% accuracy and the "optmized" model barely nudged upward to 65%. It is possible that the model is overfitted. Perhaps using fewer epochs could improve training. 