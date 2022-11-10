# Neural_Network_Charity_Analysis

## Overview of the Analysis 
Utilizing Machine Learning and Neural Networks for this project, I used the features in the Charity dataset to create a binary classifier that will assist in predicting if the applicants that will be funded by a Charitable organization, called Alphabet Soup, will be successful. 

In this analysis, I used a dataset containing various measures on 34,000 organizations that have been funded by Alphabet Soup. This project compromised of the following 3 steps: 


* Preprocessing data for the neural network 
* Compile, Train, & Evaluate the Model 
* Optimizing the model

## Results 

### Data Preprocessing 
- Variable that was considered as the target for my model: IS_SUCCESSFUL Column.
- Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop off.
- Variables that were neither targets or features for the dataset: Columns that I dropeed are EIN, NAME because they will have little to no impact om our outcome.

### Compiling, Training and Evaluating the Model

The number of neurons, layers, and activation functions I selected for my neural network model:
- For my neural network model I had 2 hidden layers. My first layer had 80 neurons, the second has 30 there is also an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/image1.png)

Was the model able to achieve the target model performance?
- The model was not able to reach the target 75%. The accuracy for my model was 71%.

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/image2.png)

The steps taken to try and increase model performance

- Attempt 1: Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same, however model accuracy went  to 71%. 

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/img2.png)


-  Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy went down again, this time it was 53%.

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/img4.png)

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/img5.png))

- Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model went down even more to 43%.

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/img6.png)

![img](https://github.com/DannyJohnson-Hi/Neural_Network_Charity_Analysis/blob/main/resources/img7.png)

## Summary 

The model ended with the accuracy score of 43% after optimization. The initial neural network had an accuracy score of 71%. This loss in accuracy can be reflected by the fact that the model overfitted. I could also further optimize the neural network by removing more features or by adding more data to the dataset to increase accuracy.
Since my accuracy score was not particularly up to the standard with neural networks, I could have used the Random Forest classifiers. This is because random forest is a robust and accurate model due to their sufficient number of estimators and tree depth. Also the random forest models have a faster performance than neural networks and could have avoided the data from being overfitted. 
