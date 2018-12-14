# Tensorflow

Using the hand-written digit database MNIST, create a machine learning model to recognize hand-written digits. By using Tensorflow, the model was trained to recognize digits by having it "look" at thousands of examples and check the model's accuracy with the test data.

Tools: Python, Sci-kit Learn, Tensorflow, Vanilla Dense Neural Network (Vanilla DNN)

## Data:

MNIST - the most classic Neuro Network dataset

The MNIST data is split into three parts: 55,000 data points of training data (mnist.train), 10,000 points of test data (mnist.test), and 5,000 points of validation data (mnist.validation). 

Every MNIST data point has two parts: an image of a handwritten digit and a corresponding label. We'll call the images "x" and the labels "y". Both the training set and test set contain images and their corresponding labels; for example the training images are mnist.train.images and the training labels are mnist.train.labels.

## Summary: 

Use the MNIST dataset (with labelled images of digits) for training a vanilla Dense Neural Network with the following characteristics:
1. Input layer of size 784 (since each image is 28 X 28)
2. Three hidden layers of size 300,200,100
3. Output layer of size 10 (to classify digits 0-9)
4. Use Leaky Relu activation function in hidden layers (Ref:tf.nn.leaky_relu​, ​wiki​)
5. Use a dropout ratio of 10% on all hidden layers (Ref:tensorflow​, ​dropout ​)
6. Use cross entropy loss (Ref:​tensorflow​)

Train this network for classification of images of digits using MNIST data, using stochastic mini batch gradient descent for 10 epochs and batch sizes of 50 and report performance. 

Achieved a Train Accuracy of 0.96 and Validation Accuracy of 0.9614 after 10 epochs.