# Convolutional-Neural-Network

# First Architecture
The Conv2D layer creates a convolution kernel that is convolved with the layer input to produce a tensor of outputs. A ReLU activation function is used because most of the people found out that ReLU layers work far better because the network is able to train a lot faster, without making a significant difference to the accuracy, with output of volume(30,30,32) and fitter size(3,3) and 0 padding, then the pooling layer with size (2,2) the main purpose of a pooling layer is to reduce the number of parameters of the input tensor and thus helps reduce overfitting, extract representative features from the input tensor, reduces computation and thus aids efficiency. Finally the fully connected layer, the input to the fully connected layer is the output from the final Pooling or Convolutional Layer, which is flattened to a vector of size 1024 and then fed into the fully connected layer. After passing through the fully connected layers, the final layer uses the softmax activation function (instead of ReLU) which is used to get probabilities of the input being in a particular class (classification).

# Second Architecture
I used four layers with different activation function which is tanh, the advantage of it is that the zero input will be mapped near zero and the negative input will be mapped strongly negative. The accuracy achieved with patch size of 64 and epoch of size 50 is 68%.

# Third Architecture

With the third layer I used 6 layers withReLU activation function and the regularization parameter. The regularization is added to give a penalty to the loss with respect to that layer's weights which has noticeably improved the accuracy of the model with 85% accuracy.
