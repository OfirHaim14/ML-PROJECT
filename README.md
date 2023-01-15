# ML-PROJECT
ML project that goes from simple ML models to Artificail Neural Network
## Data Set:
The data set is about diamonds and was taken from Kaggle.  
The data set URL: https://shorturl.at/bgzOX. 
## Our models:
### Regression Artificial Neural Network:
Our model enables us to get a number of hidden layers from different sizes in a list. The number of hidden layers and hidden cells in every layer are the hyperparameters of the model. 
The optimizer is Adam and the loss is MSE.
#### Hyper parametrs tuning: 
The hyperparameters are learning rate, batch size, and the number of hidden layers and hidden cells in every layer. The values that gave the best performance – the minimum loss, are  Learning Rate – 0.001, Batch Size – 100, number of layers – 3, and number of cells – 15.  
After trying a lot of values of epochs, seventy-five epochs gave us the best results.
With the best hyperparameters, the results were:  
When the upper graph is the loos on the train and the other is on the validation.
![The loss on the train and validation](https://user-images.githubusercontent.com/118376368/212502295-7ac44f82-d363-4a2e-a4ed-fc57c99e0670.png)

#### Regularization:
In order to prevent Overfitting and to make the loss more stable, we added L1, L2 regularization. 

### Linear Regression:
For this model, we used Sklearn LinearRegression(). 
We found the hyperparameters and parameters by using the function Gridsearchcv().  
After finding the best params and hyper params and running the model on the test data we got the graph below.  
Because our data don’t have linear connections from all our models this had the worst results.
![predicted vs original](https://user-images.githubusercontent.com/118376368/212502565-472ce500-d6a3-46bb-bb24-fcf8d93d37be.png)


### Decision Tree Regression
For this model, we used Sklearn’s DecisionTreeRegressor().  
We found the hyperparameters and parameters by using the function Gridsearchcv().  
The graph below is of the decision tree we got. After finding the best hyperparameters we got: MSE = 0.0021980024725109576, MAE = 0.026370013007981752, R2 Score = 0.9533918564817808.  
![Decision Tree](https://user-images.githubusercontent.com/118376368/212503137-146962bc-d4bf-40e9-bfac-f19a890f59e2.png)


### Random Forest Regression
For this model, we used Sklearn’s RandomForestRegressor().   
Random Forest is practically a collection of decision trees that are being built while we train. When we want to do the regression with a random forest the model takes the average of the loss of every tree it built when the number of trees in the model is one of the hyperparameters. Because of that Random forest is more accurate that a single decision tree and prevents the single decision tree's tendency to overfit.  
We found the hyperparameters and parameters by using the function Gridsearchcv().  
After finding the best hyperparameters we got: MSE = 0.0011835961014466684, MAE = 0.01613269253007221, R2 Score = 0.9749021133261915. As expected Random forest is more accurate than a single decision Tree.

### K-Nearest Neighbors Regression:                        
For this model, we used Sklearn’s KNeighborsRegressor(). We found the hyperparameters and parameters by using the function Gridsearchcv().  After finding the best hyperparameters we got: MSE = 0.0017245582203189304, MAE = 0.02059501959897579, R2 Score = 0.9634311343852464.

# Comparing the models:

![The model and it's results](https://user-images.githubusercontent.com/118376368/212503264-4efca0a9-54cd-4022-af02-3b60f851a4ac.png)  
As expected the model with the best results is the neural network when random forest very close to him.
