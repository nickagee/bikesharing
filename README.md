# Bikesharing Prediction Project

This is a simple NN approach to predict daily bike rental ridership.

## Data

This dataset has the number of riders for each hour of each day from January 1 2011 to December 31 2012. The number of riders is split between casual and registered, summed up in the `cnt` column. You can see the first few rows of the data above.

![10 days of Ridership](assets/dataview-riders.png)
First 10 days fo ridership

## Network

The network has two layers, a hidden layer and an output layer. The hidden layer will use the sigmoid function for activations. The output layer has only one node and is used for the regression, the output of the node is the same as the input of the node. That is, the activation function is $f(x)=x$. A function that takes the input signal and generates an output signal, but takes into account the threshold, is called an activation function. We work through each layer of our network calculating the outputs for each neuron. All of the outputs from one layer become inputs to the neurons on the next layer. This process is called *forward propagation*.

![](assets/nn_train_val_loss.png)
Train/Val Loss of best Training Run.

![](assets/nn_pred.png)
Predictions