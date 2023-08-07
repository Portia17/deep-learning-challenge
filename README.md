# deep-learning-challenge
Module 21 Challenge for Data Analysis Bootcamp

## Overview of the Analysis
The purpose of this analysis was to use a neural network to classify the success of applicants to a nonprofit foundation that allocates money to different charities.  We used a dataset with information such as the type of organization, what they were using the money for, and the asking amount to train the neural network.  There were 34,299 records which was cleaned and split allowing for 75% to be used for training and 25% to be used for testing.

<img width="907" alt="Screenshot 2023-08-07 at 15 05 24" src="https://github.com/Portia17/deep-learning-challenge/assets/120141110/26695ca0-c93b-4dd8-aa78-95f723155286">

In this analysis, the target was the IS_SUCESSFUL column.  We removed the NAME and EID columns as they were not useful for our analysis.  We also wittled down the columns with too many variables so there were less options for each and classified all the uncommonly used variables as "Other".  We used the remaining columns in our analysis to train and test all four models on.

<img width="385" alt="Screenshot 2023-08-07 at 15 05 44" src="https://github.com/Portia17/deep-learning-challenge/assets/120141110/d41862ea-7554-4a9a-9814-cbde6b9d20e8">

## Results
We created four different models.  First, we made a basic model with two hidden layers using ReLU activation and an output layer using Sigmoid activation, the first layer having 100 neurons and the second having 30 and an output of 1.  The second model had four hidden layers and one output layer.  The first layer had 100 neurons, the second had 50, the third had 25, and the fourth had 10 all using ReLU activation with the output of one using Sigmoid activation. The first layer had 100 neurons, the second had 50, the third had 25, and the fourth had 10 with the output of one using Sigmoid activation and was slightly less accurate than when using ReLU.  The fourth model had five hidden layers, the first with 150 neurons, the second with 75 neurons, the third with 40 neurons, the fourth with 10 neurons, the fifth with 5 neurons all using ReLU activation and the final output using Sigmoid activation.  We ran all models for 200 epochs as accuracy usually maxed out a bit before that number.  The results were all about the same with a training accuracy of a little over 74% and a texting accuracy between 72.3% and 72.6%.  None of the models reached the desired 75% accuracy despite increasing both layers and neuron amount and trying different activation methods.

<img width="584" alt="Screenshot 2023-08-07 at 15 13 12" src="https://github.com/Portia17/deep-learning-challenge/assets/120141110/c39da678-d63d-4e7f-978a-d770ec390e9a">

## Summary
While the models performed better than chance, they were not sufficient to classify whether the charity applicants would be successful.  Despite the steps taken to optimize the model it performed similarly across all circumstances and is clearly not the right fit for this kind of analysis.


