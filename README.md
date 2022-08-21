# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis:
The loan prediction risk analysis is a project to ensure that a non profit foundation, Alphabet Soup, uses donations only towards impactful organizations where the funds will be used for the environmental causes it supports. There have been issues in the past where donations are given to organizations that improperly use the funds. The President of Alphabet Soup wants to know which organizations are worth donating to and which are too high risk so they can ensure the funds go to the right organizations.. 
The csv file, "charity_data.csv" was  used to pull all of the data for this project.

## The purpose of this analysis:
The purpose of this analysis is to make predictions to determine which organizations should receive funding and which ones should not, based on past performance.

## Results:

* What variable(s) are considered the target(s) for your model? The "IS_SUCCESSFUL" column is the taget because that tells us if the money used effectively in the past, which indicates that the is an organization that can receive the donation.

* What variable(s) are considered to be the features for your model?"APPLICATION TYPE, and NAME columns were used as the target because those names that appear numerous times and have been unsuccessful in the past would most likely be high risk, and the machine model can pick up on those patterns. 


* What variable(s) are neither targets nor features, and should be removed from the input data? The EIN number was removed rom the model because that did not provide any useful data.

* How many neurons, layers, and activation functions did you select for your neural network model, and why? There are 2 layers, the first with 80 neurons, and the 2nd has 30 neurons. The first layer uses the "relu" activation and the 2nd uses the "relu" as well. The output layer uses the "sigmoid" function. 
I did not want to use too many neurons in either layer due to the risk of overfitting.

* Were you able to achieve the target model performance? Yes, the accuracy rate of 78.8% was reached.

* What steps did you take to try and increase model performance?  I included the "NAME" column and I used ptl.xlim to narrow down the count values to use for the "NAME" counts, as well as for the application "CLASSIFICATION" to see where to separate the names into "other", so there would be less noise with unneccessary data. The first two deliverables did not include the "NAME" column.
Increasing value count of the application type from counts less than 100 to counts less than 500 captured more relevant information that the model could use for more accuracy.

The objects used in the analysis are:
['NAME',
 'APPLICATION_TYPE',
 'AFFILIATION',
 'CLASSIFICATION',
 'USE_CASE',
 'ORGANIZATION',
 'INCOME_AMT',
 'SPECIAL_CONSIDERATIONS']

## Summary:

The model produced an accuracy rate of 78.8%, which exceeds the goal of 75% accuracy. 
The current models used produced results of close to 79% accuracy, so the models used were very effective. If the results produced less than 75% accuracy, other models would have been considered.


