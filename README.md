# Neural_Network_Charity_Analysis

## Overview of the analysis:

In this analysis we are tasked to create a deep learning neural network model. We have a CSV file from Alphabet Soup containing 34,000 organizations that have received funding. We are using the dataset and creating a binary classifier to predict if an applicant will be successful if it was funded by Alphabet Soup.

## Results:

- Data Preprocessing

  - The variable that is the target is the IS_SUCCESFUL column because we are trying to see if we can predict that attribute.
  
  - The variables that are the feature variables are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATION, AND ASK_AMT.
  
  - There are two variables that are neither target or features and are removed are EIN and NAME.
  
- Compiling, Training, and Evaluating the Model

  - The total amount of neurons that was used was 110, the number layers were 2, and the activation function that I used was relu and sigmoid. The neurons that I used was double the amount of features I had in the first layer and in the second I used about half of the total in the second layer. The rule of thumb is you want to have 2 to 3 times more neurons that the number of features so that was right in between 2 and 3 times. Also, the two layers were added so it can be more efficient if I subtracted one more layer the model would not be able to compute the amount of data correctly and I did not add a third because I did not want it to potentially overfit the data. 
  
  - I was not able to achieve the target model performance of 75% the closest I was able to get was 74%.
  
  - There were many steps I took to try to increase the model’s accuracy. I increased the number of neurons to see if that would help classify the data better. Also, I checked if I added a third hidden layer if that was able to increase accuracy. Also, I changed the binning data and changed the activation function from relu to tanh to see if that helped with accuracy.

## Summary: 

The deep learning model showed that the highest accuracy number that I could get was 74% even with changing activation functions, number of neurons, and layers. I tried to use random forest to see if that would give me a better result, but the actual accuracy was less at 70%. Another option is to use an SVM model because it is less prone to overfitting and works well with tabular data.
