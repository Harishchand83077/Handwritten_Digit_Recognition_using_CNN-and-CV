# Handwritten_Digit_Recognition_using_CNN-and-CV

**Convolution Neural Network**
A Convolutional Neural Network or CNN is a Deep Learning Algorithm which is very effective in handling image classification tasks. It is able to capture the Temporal and Spatial dependencies in an image with the help of filters or kernels

The kernel is just like a small window sliding over the large window in order to extract the spatial features and in the end, we get feature maps.![cnn-sliding-kernel](https://github.com/user-attachments/assets/af29551b-0818-4798-baed-e98f03eefd2f)

**MNIST Dataset**

We are going to use the famous MNIST dataset for training our CNN model. The MNIST dataset was compiled with images of digits from various scanned documents and then normalized in size. Each image is of a dimension, 28×28 i.e total 784 pixel values.


**Layout of the basic idea**
Firstly, we will train a CNN (Convolutional Neural Network) on MNIST dataset, which contains a total of 70,000 images of handwritten digits from 0-9 formatted as 28×28-pixel monochrome images.
For this, we will first split the dataset into train and test data with size 60,000 and 10,000 respectively.
Then, we will preprocess the input data by reshaping the image and scaling the pixel values between 0 and 1.
After that, we will design the neural network and train the model.
After the model is trained, we will save it for future use.
Next, we are going to use a webcam as an input to feed an image of a digit to our trained model.
Our model will process the image to identify the digit and return a series of 10 numbers corresponding to the ten digits with an activation on the index of the proposed digit.
Download Handwritten Digit Recognition Code
Please download project source code: Handwritten Digit Recognition in Python

**File Structuring**
1. Train.py
We utilize the MNIST dataset to train our CNN model and then save the model in the current working directory.

2. RecognizeDigit.py
We load the saved model and use appropriate functions to capture video via webcam and pass it as an input to our model. Our model produces a prediction which is displayed to the user.

**Libraries Required**
Make sure that the following libraries are installed on your working machine before proceeding further

Keras
Tensorflow
OpenCV
Sklearn
Numpy
