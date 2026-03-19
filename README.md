# Skin Disease Detection

**Deep Learning Based Image Classification for Skin Health Analysis**

## Overview

This project focuses on building a deep learning model that can classify skin images as either normal or diseased. It uses transfer learning with MobileNetV2 to efficiently extract features and make accurate predictions.

The system processes input images and provides real time predictions, making it useful for early detection and analysis. This project demonstrates an end to end machine learning pipeline including data preprocessing, model training, and inference.

---

## Features

- Binary Classification  
  Classifies skin images into normal or disease categories  

- Transfer Learning  
  Uses MobileNetV2 pretrained on ImageNet for efficient feature extraction  

- Automated Data Processing  
  Splits dataset into training and validation sets automatically  

- Real Time Prediction  
  Accepts input images and outputs prediction instantly  

- Lightweight Model  
  Fast and efficient for local system usage  

---

## Demo

To see the model in action  

[![Watch Demo](https://img.youtube.com/vi/ajinucjHfJQ/0.jpg)](https://youtu.be/ajinucjHfJQ)

---

## Getting Started

### Prerequisites

- Python 3.9 or above  
- TensorFlow  
- OpenCV  
- NumPy  

### Install dependencies

pip install tensorflow opencv-python numpy matplotlib  

---

## Project Structure

normal folder contains images of healthy skin  
disease folder contains images of diseased skin  
data folder is automatically created for training and validation  
model file stores trained model  
notebook or script contains training and prediction code  

---

## How It Works

Images are resized to 224 by 224 pixels  
Pixel values are normalized between 0 and 1  
MobileNetV2 is used as the base model  
The base model is frozen to preserve pretrained features  
Custom dense layers are added for classification  
Model is trained using binary crossentropy loss  
Prediction is made using sigmoid activation  

---

## Model Performance

Training accuracy reaches high values due to transfer learning  
Validation accuracy shows strong classification capability  
Predictions return probability scores for each class  

---

## Example Output

The model outputs a probability value between zero and one  

If the value is less than zero point five the image is classified as disease  
If the value is greater than zero point five the image is classified as normal  

---

## Limitations

The model is trained on a limited dataset  
May not generalize well to all real world skin conditions  
Not suitable for medical diagnosis  

---

## Future Improvements

Add data augmentation for better generalization  
Train on larger and more diverse datasets  
Fine tune the base model  
Deploy as a web application  

---

## Author

Chehal Minocha
