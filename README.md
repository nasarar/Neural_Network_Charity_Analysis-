# Neural_Network_Charity_Analysis


## Project Overview
A deep neural network's binary classification model is used in order to quanitfy which of Alphabet Soup's applicants are considered worth donating to and which ones are high risk. 

## Resources
-Data Source: charity_data.csv

## Results
-Data Preprocessing:
  - The 'IS_SUCCESSFUL' column from the dataset is the target for the model.
  - The features includes all columns except for 'IS_SUCCESSFUL', 'SPECIAL_CONSIDERATIONS_N', and 'SPECIAL_CONSIDERATIONS_Y' columns
  - The 'EIN' and 'NAME' columns were expected to be non-essential to the model and was therefore removed.

-Compiling, Training, and Evaluating the Model:
  - There are 3 hidden layers towards the model with 80 neurons in the first layer, 40 neurons in the second layer, and lastly 20 neurons in the third layer.
  - The model was able to only reach 72% accuracy from the targetted 75%.
  - There are three big steps that was taken in order to increase the model performance. First, the dataset was cleared of more 'noise' and based on the testing, the 'SPECIAL_CONSIDERATIONS_N', and 'SPECIAL_CONSIDERATIONS_Y' columns made little to no difference on the model.
  ![](/Resources/combination.png)
  
  The second step was adding another hidden layer with 20 neurons and a Relu activation function. 
  ![](/Resources/hidden_layer.png)
  
  Lastly, more epochs were added to the model from 50 to 100 epochs.
  ![](/Resources/epochs.png)
  
  
## Summary
Although, the neural network performs very well in complex and large datasets. Sometimes, it might be more efficient to perform simple models from supervised and unsupervised machine learning. For the projects next step, I would try to use the Random Forest Classifier with the current dataset and check if the results is the same or relatively similar. If so, I would use the Random Forest model to classify the low and high risk funding since it would be less complicated to read, and would take less time to run.  
