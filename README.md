# Human-Action-DNN
In this project, I will be making a CNN in order to predict human actions in images.  Using a massive dataset found on kaggle: https://www.kaggle.com/datasets/emirhanai/human-action-detection-artificial-intelligence, 
I will traing the CNN. More details on the architecture are below.  

The goal of this is to create the framework for a CNN I can use for real-time running form analysis. Since the massive explosion of runners, my collegues and I are working on an application that will replace PT for runners. Utilizing this CNN, we hope to implement it to find errors in running form.  


### Loading the Data

First, I will load my data and transform them to Tensors for PyTorch readability. I will define my transformations as follows.

### Defining the model

I will create a simple CNN with this architecture:
- Convolutional Layer
- ReLu for the activation function
- MaxPooling for the pooling layer
- Fully connected layer
- And softMax for the output activation

### Optimizer and Loss Function
I will now define the optimizer, and Losws function.  I will use cross entropy loss for the loss function, and Adam for the optimizer with a learning rate of 0.001.  I will also add on an accuracy test to print out the accuracy during training.

### Predicting Custom Images
I will now make a simple function that I can use to predict the action on simple images.  This will be adjusted consistently 