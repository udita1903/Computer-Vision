
# Image Classification on Fashion MNIST

This repository contains a Convolutional Neural Network (CNN) model implemented using TensorFlow and Keras for image classification tasks. The model is designed to classify images into one of ten categories and can be particularly useful for tasks like digit recognition or object classification.


# About Dataset

Fashion-MNIST is a dataset comprising of 28×28 grayscale images of 70,000 fashion products from 10 categories, with 7,000 images per category. The training set has 60,000 images and the test set has 10,000 images. Fashion-MNIST shares the same image size, data format and the structure of training and testing splits with the original MNIST.


# Model Architecture
Convolutional Layers:The model begins with two convolutional layers, each followed by a max-pooling layer. These layers are responsible for extracting important features from input images.
Flatten Layer:
 After the convolutional layers, the Flatten layer is used to transform the 2D feature maps into a 1D vector, preparing the data for fully connected layers.
Fully Connected Layers: The model includes two fully connected dense layers. The first dense layer with 128 units and ReLU activation functions is used to learn complex patterns from the flattened data. The final dense layer with 10 units and a softmax activation function provides the output probabilities for each of the ten categories.

# Model Training
Optimizer: The model is trained using the Adam optimizer, which is known for its efficiency in optimizing deep neural networks.
Loss Function: The loss function used is 'sparse_categorical_crossentropy,' suitable for multi-class classification tasks.
Training Data: The model is trained on a dataset consisting of training images (xtrain) and their corresponding labels (ytrain).
Epochs: The training process consists of 20 epochs, allowing the model to learn and improve its performance over time.
