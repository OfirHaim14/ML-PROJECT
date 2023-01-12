# ML-PROJECT
ML project that from ML simple models to Artificail Neural Network
# Data Set:
The data set is about diamonds and was taken from Kaggle. The data set URL: https://shorturl.at/bgzOX. 
# Our models:
## Regression Artificial Neural Network
Our model enable us to get a number of hidden layers from different sizes in a list. The number of hidden layers and hidden cells in every layer are the hyper parametrs of the model. 
The optimizer is Adam and the loss is MSE.
Hyper parametrs tuning:
The hyper parametrs are learning rate, batch size and the number of hidden layers and hidden cells in every layer. The values that gave the best perforemnces – the minimum lost are 
Learning Rate – 0.001, Batch Size – 100, number of layers – 3, number of cells – 15. 
After trying a lot of values of epochs, sventy five epochs gave us the best results.
With the best hyper parametrs the results were:
When the upper graph is the loos on train and the other is on the validation.





In order to prevent Overfitting and to make the loss more stable, we added L1, L2 regularization. 
Lambada1 is the name for L1 regularization lambda and Lambada2 is the name for L2 regularization lambda. 
The results for each lanbda values:


 

