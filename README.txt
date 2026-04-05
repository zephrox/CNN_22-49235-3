# Facial Expression Recognition using CNN (FER-2013)

## Overview

This project implements a Convolutional Neural Network (CNN) to classify facial expressions using the FER-2013 dataset. The goal is to build a custom CNN model, train it, and evaluate its performance on multiple emotion classes.

## Dataset

* Dataset: FER-2013 (Facial Expression Recognition)
* Classes:

  * Angry
  * Disgust
  * Fear
  * Happy
  * Sad
  * Surprise
  * Neutral
* Images are grayscale and resized to 48×48 pixels.

## Methodology

### Data Processing

* Dataset loaded using Hugging Face `datasets`
* Train, validation, and test splits created
* Data augmentation applied:

  * Random horizontal flip
  * Small rotations
* Images normalized for stable training

### Model Architecture

Two CNN models were designed:

1. **Baseline CNN**

   * Simple convolutional layers
   * No regularization

2. **Improved CNN**

   * Batch Normalization
   * Dropout layers
   * Better generalization

### Training

* Loss function: CrossEntropyLoss
* Optimizer: Adam
* Learning rate scheduling used
* Best model saved based on validation accuracy

## Results

* Training and validation accuracy plotted
* Confusion matrix generated
* Classification report (Precision, Recall, F1-score)
* Per-class performance analyzed

## Key Observations

* Some emotions like *Happy* are easier to classify
* Confusion occurs between similar expressions like *Fear* and *Surprise*
* Regularization (BatchNorm + Dropout) improves performance

## How to Run

1. Open the notebook in Google Colab
2. Enable GPU (Runtime → Change runtime type → GPU)
3. Run all cells

## Files

* `CNN_StudentID.ipynb` — main notebook
* `best_fer2013_model.pth` — trained model weights

## Conclusion

A custom CNN was successfully trained on the FER-2013 dataset. The improved model achieved better generalization and performance. Future work could include transfer learning and deeper architectures.
