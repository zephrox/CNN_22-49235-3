# Facial Expression Recognition using CNN (FER-2013)

## Project Overview
This project is a facial expression recognition system built using a custom Convolutional Neural Network (CNN). The model is trained on the FER-2013 dataset to classify grayscale face images into 7 emotion categories.

The main goal of this work is to design, train, and evaluate a CNN model for image classification, while also analyzing its strengths and weaknesses through proper evaluation metrics and visualizations.

## Dataset
The dataset used in this project is **FER-2013 (Facial Expression Recognition)**.

It contains face images of size **48 x 48** in grayscale.  
The model classifies each image into one of the following 7 classes:

- Angry
- Disgust
- Fear
- Happy
- Sad
- Surprise
- Neutral

## What was done in this project
In this notebook, the following tasks were completed:

- Loaded and explored the dataset
- Applied preprocessing and data augmentation
- Created training, validation, and test data loaders
- Built custom CNN architectures
- Compared a baseline CNN and an improved CNN
- Trained the model using Adam optimizer
- Used learning rate scheduling
- Evaluated the model using accuracy, precision, recall, and F1-score
- Plotted training/validation loss and accuracy curves
- Generated a confusion matrix
- Saved the best model weights

## Model Summary
The final model is a custom CNN with:
- convolution layers
- batch normalization
- ReLU activation
- max pooling
- dropout for regularization
- fully connected layers for classification

## Results
The final model achieved around **60% validation accuracy** on the FER-2013 dataset.

The model showed steady improvement during training, and the learning rate scheduler helped improve validation performance after the model began to plateau.

## Files
- `CNN_22_49235_3.ipynb` → main notebook
- `best_fer2013_model.pth` → saved trained model
- `README.md` → project documentation

## How to run
1. Open the notebook in Google Colab or VS Code
2. Install the required libraries
3. Run all cells from top to bottom
4. The best model will be saved automatically during training

## Conclusion
This project shows how a custom CNN can be used for facial expression recognition. Although the dataset is challenging, the model was able to learn useful visual features and achieve reasonable performance. Future improvements could include transfer learning, deeper architectures, and more tuning of hyperparameters.