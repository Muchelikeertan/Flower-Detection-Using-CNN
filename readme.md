# Flower Detection Using CNN

A deep learning project that classifies flower images into **5 different categories** using a Convolutional Neural Network (CNN) built with **TensorFlow and Keras**.

## Project Objective

The objective of this project is to build a CNN model capable of identifying the category of a flower from an input image.

## Dataset

The project uses the **5 Flower Types Classification Dataset** available on Kaggle.

The dataset is downloaded using KaggleHub.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- KaggleHub

## Data Preprocessing

The images are:

- Resized to `224 × 224` pixels
- Normalized using pixel values divided by `255`
- Divided into:
  - 80% training data
  - 20% validation data

## CNN Architecture

The model consists of:

1. Conv2D layer - 32 filters
2. MaxPooling2D
3. Conv2D layer - 64 filters
4. MaxPooling2D
5. Conv2D layer - 128 filters
6. MaxPooling2D
7. Flatten layer
8. Dense layer - 128 neurons
9. Output layer - 5 neurons with Softmax activation

## Model Configuration

- Optimizer: Adam
- Loss Function: Categorical Cross-Entropy
- Evaluation Metric: Accuracy
- Training Epochs: 6
- Batch Size: 32

## Prediction

After training, the model can be used to classify a new flower image.

The input image is resized to `224 × 224`, normalized, and passed to the trained CNN model. The class with the highest prediction probability is returned as the predicted flower category.

## Project Workflow

Dataset  
↓  
Preprocessing  
↓  
Training/Validation Split  
↓  
CNN Model  
↓  
Model Training  
↓  
Model Saving  
↓  
New Image  
↓  
Prediction

## Model File

The trained model is saved as:

`FLower_detection.h5`

## Notebook

The complete implementation is available in:

`Flower_Detection_model_Using_CNN.ipynb`
