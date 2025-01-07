Vietnamese Handwritten Recognition with CRNN Model
Project Overview
This project implements a Vietnamese handwritten text recognition system using the CRNN (Convolutional Recurrent Neural Network) model. The system is designed to accurately detect and recognize handwritten Vietnamese characters in scanned images or photographs, addressing challenges such as variations in handwriting styles, inconsistent spacing, and noise.

Key Features
Handwriting Recognition: Detect and recognize Vietnamese text from handwritten input.
CRNN Architecture: Combines convolutional layers for feature extraction and recurrent layers for sequential data processing.
End-to-End Pipeline:
Preprocessing raw image data.
Model training and evaluation.
Predicting and visualizing handwritten text.
Vietnamese Language Support: Handles accents and unique characters in the Vietnamese script.
Dataset
The project uses a dataset of Vietnamese handwritten text images. Each image is labeled with the corresponding text. The dataset is split into:

Training Set: Used to train the model.
Validation Set: Used for hyperparameter tuning.
Test Set: Used for final model evaluation.
Preprocessing Steps:

Grayscale conversion.
Normalization.
Resizing to a fixed height while maintaining aspect ratio.
Model Architecture
The CRNN model is designed for sequence-to-sequence learning:

Convolutional Layers: Extract spatial features from the image.
Recurrent Layers (RNN): Process sequential data from the convolutional output.
CTC Loss: Optimizes the model to align predicted sequences with the ground truth without requiring frame-level labels.
