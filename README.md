## Utilizing machine learning and neural networks to predict whether applicants of Alphabet Soup's Non-Profit Foundation will be successful


#### Overview of the analysis: 

The purpose of this analysis is to develop a binary classifier using machine learning and neural networks to predict the success of organizations funded by Alphabet Soup.The dataset is preprocessed to identify target and feature variables (dropping unnecessary columns), encoding categorical variables, and splitting the data into training and testing sets. The neural network model was trained but the outcome was subpar. To achieve a target predictive accuracy higher than 75% I developed optimization strategies including adjusting input data, modifying network architecture, and experimenting with different activation functions and training epochs. The optimized model exceeded the accuracy goal of 75%, receiving a 79.2% accuracy. 

Results: Using bulleted lists and images to support your answers, address the following questions:

#### Data Preprocessing

What variable is the target for your model?
  - The target variable (y) for the experiment is the IS_SUCCESSFUL

What variable(s) are the features for your model?
 - The feature variables (X) for the experiment are: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

What variable should be removed from the input data because they are neither targets nor features?
 - The EIN and NAME features were initally removed to aid the model

#### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions were selected for your neural network model, and why?
 - I initiated with a configuration of two layers, assigning 3 neurons to the first layer and 6 to the second, based on intuition. Observing an accuracy hovering around the 70% mark, I proceeded to experiment with different combinations. Despite various attempts, the highest accuracy I managed to attain was 72%, achieved with a setup comprising two layers with 9 and 18 neurons, respectively.

Were you able to achieve the target model performance? 
  - I successfully attained the target performance threshold of 75% or higher, achieving a notable accuracy rate of 79.2% through three distinct optimization approaches.

What steps did you take in your attempts to increase model performance?
Initially, I reintroduced the "NAMES" column into my model as a starting point. I experimented with various configurations, starting with my previous settings of 9 layers with 18 neurons, and applied binning to names with thresholds set at < 10 and then < 5. Observing a greater percentage increase with the < 5 threshold, I retained this approach. Subsequently, I iteratively adjusted the layers, neurons, and activation functions. Ultimately, I achieved a 79.2% accuracy across three distinct models:
  - A two-layer model with 10 and 20 neurons respectively, utilizing ReLU activation.
  - A two-layer model with 10 and 20 neurons respectively, utilizing tanh activation.
  - A three-layer model with 15, 30, and 45 neurons respectively, using tanh, tanh, and ReLU activation functions.

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
