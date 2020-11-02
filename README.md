# Neural Network Charity Analysis

## Project Overview 
Becks is a data scientist and programmer for the nonprofit foundation Alphabet Soup. They are a philanthropic foundation dedicated to helping organizations that protect the environment, improve people's well-being, and unify the world. Alphabet Soup has raised and donated over 10 billion dollars in the past 20 years. this money has been used in lifesaving technologies and organizes reforestation groups around the world. Beck is in charge of data collection and analysis for the entire organization. Her job is to analyze the impact of each donation and vet potential recipients. This helps ensure that the foundation's money is being used effectively. Unfortunately, not every donation the company makes is impactful. In some cases, an organization will take the money and disappear. As a result, Alphabet Soup president Andy Glad has asked Becks to predict which organization is worth donating to and which are too high risk. Alphabet Soup’s business team provided Beks with a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The purpose of the project is to use the features in the provided dataset to help Becks create a robust deep learning neural network capable of interpreting large complex datasets that will help Becks and Alphabet Soup determine which organizations should receive the donation.

## Results
### Data Preprocessing
What variable(s) are considered the target(s) for your model?
> Target variable(s): IS_SUCCESSFUL 

What variable(s) are considered to be the features for your model?
> Features variable(s): APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, STATUS

What variable(s) are neither targets nor features, and should be removed from the input data?
> Removed variable(s): EIN, NAME

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
> Layer | Neurons | Activation function
> -----| -----|-----
> First hidden| 80 | relu
> Second hidden |30 | relu
> Output |  | Sigmoid

> Above neurons and activation functions were chosen to optimize the neural network model. 

Were you able to achieve the target model performance?
> No, the highest accuracy for the model was 71%. Our target was 75%.

What steps did you take to try and increase model performance?
> Following steps were taken to try and increase model performance: 
> - Adjusting the input data by dropping the STATUS variable
> - Added more neurons to a hidden layer.
> - Added hidden layer.
> - Used different activation functions for the hidden layers.
> - Change model's weights to be saved every 5 epochs

# Summary
The deep learning model for the alphabet soup was only able to predict 71% of the outcomes correctly at maximum. The Random forest classifiers model can be used to solve the classification problem. Random forest classifiers are a type of ensemble learning model that combines multiple smaller models into a more robust and accurate model. Random forest models have been a staple in machine learning algorithms for many years due to their robustness and scalability. Both output and feature selection of random forest models are easy to interpret, and they can easily handle outliers and nonlinear data.
