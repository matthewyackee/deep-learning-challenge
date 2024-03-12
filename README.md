# deep-learning-challenge
UofD Data Analysis Bootcamp Module 21 Challenge

The primary file is: <Alphabet_Soup.ipynb>. The <Models> directory contains the .h5 files created using the original file and the optimization attempts located in the <Optimizations> directory. The <Resources> directory contains a copy of the <charity_data.csv> utilized by the script.

I used the format provided by the Starter-Code files provided.

# Report

## Overview of the analysis:
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. Using machine learning and neural networks, the features in the provided dataset can be used to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Results:
Target value: IS_SUCCESSFUL
Irrelevant values dropped: EIN, NAME
Binned values: APPLICATION_TYPE, CLASSIFICATION
Remaining values: AFFILIATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

Two hidden layers were used for the model.
First run utilized relu, second used LeakyReLU, and third run used tanh
### Loss/Accuracy
1: .5941/.7254 relu
2: .5514/.7300 LeakyReLU
3: .5533/.7325 tanh

## Summary:
While the model comes close to the target, it does not meet the goal of 75% accuracy. Adding a third hidden layer, adjusting the neuron counts, or auto-optimization might help improve the model. The data set could also be analyzed for potential further cleaning.
