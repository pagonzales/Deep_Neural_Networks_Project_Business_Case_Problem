# Deep Neural Network Project (Classification Problem: Analysis of Audiobook customers)
## Problem
The input data represent 2 years worth of engagement. From a given database of an Audiobook app, each customer has purchased at least once. We want to create a machine learning algorithm that can predict if a customer will buy again from the audiobook company. The main idea is that the company shouldn't spend its advertising budget targeting individuals who are unlikely to come back.

## Project Objective
To create a machine learning algorithm using deep neural networks that can predict if a customer will likely to buy again or not.

## Data used
- <a href = "https://github.com/pagonzales/Deep_Neural_Networks_Project_Audiobook_Analysis/blob/main/Audiobooks_data.csv">Dataset</a>

## Metrics
- Which are the most important metrics for a customer to come back.
  - Does the customer leave a review or now?
  - What is the rating of the review?
  
## Action plan
- Preprocess the data
  - Balance the datasheet
  - Divide the dataset into train, validation, and test data
    (Standardize the data, then Shuffle it, finally split the data into 3 parts with 80%,10%,10% partition)
  - Save the data into a tensor friendly format
- Create the Machine Learning Algorithm
  - Model the data using the following parameters and hyperparameters
    - The input size is 10 (for the rating)
    - The output size is 2 (buy or not buy)
    - The hidden layer of the NN is 50 units
    - We use the "relu" activation function for the layers
    - And "softmax" activation function for the output
    - For the model fitting we use 100 epochs with 100 batch size.
    - Also, we use "early stopping" for the validation accuracy with "patience" of 2
- Finally, Test the model using the test data

## Project Insights
- Using the parameters and hyperparameters mentioned above, we found out that:
  - The accuracy of the model using the train and validation dataset is 83.45%
- After running the test dataset we found that the model has an accuracy of 80.36%
## Final conclusion
- Using the parameters and hyperparameters above, we have a test model accuracy of 80.36%. Of course, this can still be improved by altering the parameters and choosing different activation functions and hidden layers. But this model we have presented here predicts that for 10 customers we can predict that 8 of them will buy again.
