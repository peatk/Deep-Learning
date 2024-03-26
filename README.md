# Deep Learning & Neural Networks
Utilizing machine learning and neural networks to predict whether applicants of Alphabet Soup's Non-Profit Foundation will be successful


#### Overview of the analysis: 

The purpose of this analysis is to develop a binary classifier using machine learning and neural networks to predict the success of organizations funded by Alphabet Soup.The dataset is preprocessed to identify target and feature variables (dropping unnecessary columns), encoding categorical variables, and splitting the data into training and testing sets. The neural network model was trained but the outcome was subpar. To achieve a target predictive accuracy higher than 75% I developed optimization strategies including adjusting input data, modifying network architecture, and experimenting with different activation functions and training epochs. The optimized model exceeded the accuracy goal of 75%, receiving a 79.2% accuracy. 

Results: Using bulleted lists and images to support your answers, address the following questions:

#### Data Preprocessing

What variable is the target for your model? 
  The target variable (y) for the experiment is the IS_SUCCESSFUL

What variable(s) are the features for your model?
  The feature variables (X) for the experiment are: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

What variable should be removed from the input data because they are neither targets nor features?
  The EIN and NAME features were initally removed to aid the model

#### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why? To begin I 

Were you able to achieve the target model performance?

What steps did you take in your attempts to increase model performance?

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
