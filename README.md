# PredictingFromImages
mahady research academy's assignment 2

# why we need to do normalization (preprocessing of input data)
Normalization is a technique where we adjust the input data to have a mean of zero and a standard deviation of one (or scale the data to a specific range like 0 to 1). 
- to ensure that the neurons of the neural network are fed with a consistent range of data [0-1] ( consistent range means training process of model is more stable)
- without normalization some features might dominate other features due to their scale, also normalization helps algorithms like gradient descent to perform more efficeintly
- This allows for faster convergence of the model, meaning the model will be more accurate with less no of epoch training
- 
# why we need to do one hot encoding?
One-hot encoding converts these numeric labels into binary vectors where each class is represented as a unique vector with a single high (1) value and all others low (0). This prevents the neural network from assuming any ordinal relationship between classes.

basically suppose that we have a cifar dataset where each class has values like 1, 2, 3, ... al the way to 100.
now it's still important for us to convert these labels into categorical data by doing one hot encoding.
one hot encoding basically prevents the model from thinking there is any ordinal relationship betwenn the labels. Eg: the model might think class no. 99 is more important than class no.1 if one hot encoding is not done.

