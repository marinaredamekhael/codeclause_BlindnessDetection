# APTOS 2019 Blindness Detection using ResNet50

Diabetic retinopathy is a leading cause of blindness for people with diabetes and visually impaired around the world. Early detection and intervention can significantly reduce the risk of blindness. This repository contains a deep learning solution that helps in the automated detection of diabetic retinopathy stages using fundus photographs.

## Overview

This project uses the APTOS 2019 Blindness Detection dataset from Kaggle to train a ResNet50 model, a deep residual neural network, to classify the severity of diabetic retinopathy on a scale of 0 to 4:

- 0 - No DR
- 1 - Mild
- 2 - Moderate
- 3 - Severe
- 4 - Proliferative DR

## Structure

- **Data Exploration**: Visualize the data distribution and sample images.
- **Data Preprocessing**: Prepare images for model training, including augmentation.
- **Model Definition & Training**: Use the ResNet50 architecture with transfer learning.
- **Model Evaluation**: Check the model's performance on validation data.
- **Prediction**: Predict the severity level of diabetic retinopathy for a test image.

## How to Run

1. Ensure you have all required packages installed.
    ```bash
    pip install tensorflow keras pandas seaborn matplotlib opencv-python-headless
    ```

2. Set up Kaggle API credentials. Ensure you've downloaded your `kaggle.json` file from your Kaggle account settings page.

3. Clone the repository and run the notebook:
    ```bash
    git clone [YOUR_REPOSITORY_LINK]
    cd [YOUR_REPOSITORY_DIRECTORY]
    jupyter notebook
    ```

## Results

The model uses a combination of transfer learning (with ResNet50 as the base model) and a dense layer to classify images into one of five classes of diabetic retinopathy severity. With the current setup, the model achieves an accuracy of `76% & 65%` on the validation set.


## Acknowledgements

- APTOS 2019 Blindness Detection dataset: [Kaggle Dataset](https://www.kaggle.com/c/aptos2019-blindness-detection)
- ResNet50 model architecture and pre-trained weights: [Keras Applications](https://keras.io/api/applications/)
