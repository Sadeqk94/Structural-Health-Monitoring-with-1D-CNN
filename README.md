# Structural-Health-Monitoring-with-1D-Convolutional-Neural-Networks

Overview

This repository presents a 1D-Convolutional Neural Network (CNN) designed for Structural Health Monitoring (SHM) using acceleration records from the Qatar University Grand Simulator (QUGS). The QUGS dataset consists of 31 classes, comprising 30 damaged scenarios and one undamaged scenario. The CNN is developed to classify these scenarios, aiding in the detection of structural damage.

Dataset

The dataset includes acceleration records representing various structural conditions simulated by QUGS. Each scenario is for a specific structural health state.

Code Structure

    Data Loading and Preprocessing: The code fetches the QUGS dataset, applies window of 0.5 S to create one sample, splits it into training and testing sets, and prepares the data for training the CNN.

    Model Architecture: The CNN architecture is tailored for capturing patterns indicative of structural damage. It includes 1D convolutional layers for feature extraction and fully connected layers for classification.

    Training and Evaluation: The model is trained on the labeled data and evaluated using metrics such as accuracy, precision, recall, F1 score, and a confusion matrix.

    Performance Visualization: Functions for plotting the learning curve and confusion matrix are provided to visualize the model's training progress and performance.

Requirements

Ensure the following dependencies are installed:

    NumPy
    pandas
    scikit-learn
    Keras
    Matplotlib
    gdown

Usage

To run the code, set up a Python environment with the required dependencies (google colab is recommended). Execute the code to train the model, assess its performance, and apply it to new structural health scenarios.
