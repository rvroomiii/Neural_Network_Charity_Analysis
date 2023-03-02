# Neural_Network_Charity_Analysis

## Overview of the analysis:
### To help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results:
### What variable(s) are considered the target(s) for your model?
* After processing the data, the IS_SUCCESSFUL variable was created and used as the basis of the modeling.

What variable(s) are considered to be the features for your model?
* After removing 'EIN' and 'NAME', 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS' were all used as features for the modeling.
<br>![variable](/images/features.png)<br>
What variable(s) are neither targets nor features, and should be removed from the input data?
* As stated above, the 'EIN' and 'NAME', were niether targets or features and needed to be removed.

How many neurons, layers, and activation functions did you select for your neural network model, and why?
* In order to fully optimize the modeling process to achieve optimal performance, I employed the use of keras tuner.  After sixty trials, it was found that the best activation function is relu using six layers.<br>
![Best results](/images/best_config.png)
![Trial results](/images/trial_results.png)

Were you able to achieve the target model performance?
* I was unable to achieve the goal of more than 75%.  The best performance achieved yeilded a result of 0.7282.<br>
![Top three](/images/top_three.png)


What steps did you take to try and increase model performance?
* I would review the data to ensure that there are enough data points.
* Locate other data sources that might provide more acurate data.
* Locate data with more unique values

## Summary: 
### The ability to utilize a tool like keras_tuner allows for faster trials, which hones the ability of the machine learning faster.  In the case of this project, I think better data would allow for better model performance.