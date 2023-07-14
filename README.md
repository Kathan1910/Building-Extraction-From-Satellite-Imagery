# Building Extraction from Satellite Imagery

This project focuses on developing a deep learning model using TensorFlow and Keras for the extraction of buildings from satellite imagery.

## Problem Statement

The goal of the project is to accurately identify and extract buildings from satellite imagery. Building extraction from satellite imagery plays a crucial role in various applications such as urban planning, disaster management, and environmental monitoring.

## Architecture of the Project

The project follows the following steps:

## 1. Import Libraries

Import the necessary libraries such as TensorFlow, Keras, and OpenCV (cv2).

## 2. Data Loading

Load the image data and corresponding mask data from the specified directory.

## 3. Dataset Preparation

- **Sample Selection:** Take a sample of 6000 images from the dataset for training and evaluation.
- **Data Arrangement:** Arrange the image and mask data in a compatible format, ensuring alignment between the imagery and corresponding building masks.

## 4. Train-Test Split

Split the dataset into training and testing subsets to evaluate the model's performance.

## 5. Building UNet Model

- **Encoder-Decoder Architecture:** Implement the UNet architecture by dividing the encoder and decoder into blocks.
- **Model Compilation:** Compile the model with appropriate loss functions and optimization algorithms.

## 6. Model Training

- Train the UNet model on the training set using the compiled model with a predefined number of epochs (e.g., 5).
- Monitor the training process and track the training and validation accuracy and loss at each epoch.
- Visualize the training and validation accuracy and loss using plots.

## 7. Model Evaluation

- Evaluate the trained model's performance using metrics such as Intersection over Union (IoU) score.
- Calculate the IoU score to assess the accuracy of building extraction, achieving a result of 63%.

## 8. Prediction and Visualization

- Utilize the trained model to predict building masks on unseen satellite images.
- Visualize the predicted building masks overlaid on the satellite imagery for visual assessment.

## Usage

1. Prepare your satellite imagery dataset and corresponding masks in the desired directory structure.
2. Import the necessary libraries as mentioned above.
3. Load the image and mask data from the specified directory.
4. Sample 6000 images from the dataset for training and evaluation.
5. Arrange the image and mask data to ensure alignment.
6. Split the dataset into training and testing subsets.
7. Build the UNet model with encoder-decoder architecture.
8. Train the model for 5 epochs using the training set.
9. Plot and analyze the training and validation accuracy and loss.
10. Evaluate the model's performance using the IoU score.
11. Utilize the trained model to predict building masks on new satellite images.
12. Visualize the predicted masks overlaid on the satellite imagery.
