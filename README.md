# Skin Disease Detection using Deep Learning
## Overview

**This project is a binary image classification system that predicts whether a skin image is normal or shows signs of disease. The model is built using transfer learning with MobileNetV2 and trained on a custom dataset of labeled skin images.**

##Project Description

The system takes an input image and classifies it into one of two categories:

-Normal skin
-Diseased skin

The model is trained using a dataset organized into two folders named normal and disease. The images are automatically split into training and validation sets. A pretrained convolutional neural network is used to extract features and a custom classification layer is added on top.

##Technologies Used

-Python
-TensorFlow and Keras
-OpenCV
-NumPy
-MobileNetV2 pretrained model

##How the Model Works

-Images are resized to 224 by 224 pixels
-Pixel values are normalized between 0 and 1
-MobileNetV2 is used as a base model with pretrained weights
-The base model is frozen to retain learned features
-Custom dense layers are added for classification
-The model is trained using binary crossentropy loss
-Predictions are made using a sigmoid activation function

##Dataset Structure

*The dataset should be organized in the following format:*

-normal folder contains images of healthy skin
-disease folder contains images of diseased skin

The script automatically creates train and validation directories and splits the dataset into 80 percent training and 20 percent validation data.

#How to Run the Project

-Step 1 Install dependencies
pip install tensorflow opencv python numpy matplotlib

-Step 2 Place your dataset
Create two folders named normal and disease in the project directory and add images accordingly

-Step 3 Train the model
Run the training script or notebook to preprocess data and train the model

-Step 4 Save the model
The trained model will be saved as a file

-Step 5 Test the model
Place a test image in the project folder and update the file name in the prediction script
Run the prediction code to get output

##Example Output

The model outputs a probability value between zero and one

-If the value is less than zero point five the image is classified as disease
-If the value is greater than zero point five the image is classified as normal

##Project Features

-End to end machine learning pipeline
-Automatic dataset splitting
-Transfer learning using MobileNetV2
-Fast and efficient training
-Real time image prediction

##Limitations

-The model is trained on a limited dataset
-Results may not generalize to all skin conditions
This project is for educational purposes only and should not be used for medical diagnosis

##Future Improvements

-Add data augmentation for better generalization
-Train on a larger and more diverse dataset
-Fine tune the base model for improved accuracy
-Deploy as a web application for real time usage

##Author
Chehal Minocha

[![Watch Demo](https://img.youtube.com/vi/ajinucjHfJQ/0.jpg)](https://youtu.be/ajinucjHfJQ)
