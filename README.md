# ML-PROJECT
ML project that goes from simple ML models to Artificail Neural Network
## Data Set:
The data set is about diamonds and was taken from Kaggle. 
The data set URL: https://shorturl.at/bgzOX. 
## Our models:
### Regression Artificial Neural Network
Our model enables us to get a number of hidden layers from different sizes in a list. The number of hidden layers and hidden cells in every layer are the hyperparameters of the model. 
The optimizer is Adam and the loss is MSE.
#### Hyper parametrs tuning: 
The hyperparameters are learning rate, batch size, and the number of hidden layers and hidden cells in every layer. The values that gave the best performance – the minimum loss are  Learning Rate – 0.001, Batch Size – 100, number of layers – 3, and number of cells – 15.  
After trying a lot of values of epochs, seventy-five epochs gave us the best results.
With the best hyperparameters, the results were:
When the upper graph is the loos on the train and the other is on the validation.
![The loss on the train and validation](https://user-images.githubusercontent.com/118376368/212502295-7ac44f82-d363-4a2e-a4ed-fc57c99e0670.png)

#### Regularization:
In order to prevent Overfitting and to make the loss more stable, we added L1, L2 regularization. 
Lambada1 is the name for L1 regularization lambda and Lambada2 is the name for L2 regularization lambda. 
The results for each lambda value:?

### Linear Regression:
For this model, we used Sklearn LinearRegression(). 
We found the hyperparameters and parameters by using the function Gridsearchcv(). 
After finding the best params and hyper params and running the model on the test data we got the graph below. Because our data don’t have linear connections from all our models this had the worst results.
![predicted vs original](https://user-images.githubusercontent.com/118376368/212502565-472ce500-d6a3-46bb-bb24-fcf8d93d37be.png)
