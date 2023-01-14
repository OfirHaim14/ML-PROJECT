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


#### Regularization:
In order to prevent Overfitting and to make the loss more stable, we added L1, L2 regularization. 
Lambada1 is the name for L1 regularization lambda and Lambada2 is the name for L2 regularization lambda. 
The results for each lambda value:



 

