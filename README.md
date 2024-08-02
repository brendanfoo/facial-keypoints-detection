# Facial Keypoints Detection Project

# Project Overview
This Jupyter notebook presents a project on facial keypoint detection. Facial keypoints are crucial features on a face, such as the corners of the eyes, the tip of the nose, and the mouth corners. Detecting these points accurately is essential for various applications in computer vision, including facial recognition, emotion detection, and augmented reality.

# Introduction
The goal of this project is to build a model that can detect key facial points in images. These keypoints can be used for a variety of applications, from enhancing security features to improving user interaction in apps.

# Dataset
The dataset used in this project consists of facial images with annotated keypoints. Each image in the dataset has corresponding keypoints that denote significant facial features.

# Data Preprocessing
This project primarily focused on data augmentation after discovering the initial dataset contained large amounts of missing values. Techniques we used included rotation, scaling, and flipping to improve the quantity, quality, and diversity of the training set.

# Model Architecture
A convolutional neural network (CNN) was employed. The architecture includes:
- Convolutional layers for feature extraction
- Pooling layers to reduce spatial dimensions
- Fully connected layers for final keypoint prediction

# Model Training
The model is trained using the annotated dataset. Key aspects of the training process include:
- Loss Function: Mean Squared Error (MSE) is used to measure the difference between predicted and actual keypoints.
- Optimizer: Adam optimizer is employed for efficient gradient descent.
- Batch Size and Epochs: The model is trained with a specific batch size and number of epochs to ensure convergence.

# Evaluation
The model's performance is evaluated using metrics such as:
Mean Squared Error (MSE) on the validation set
Visual inspection of predicted keypoints on sample images

# Results
We learnt from our different models that it was important to focus on the quality of the training data rather than just the quantity, where less training data that was more accurate was more useful than more data with null values. It would then be valuable to pursue more data augmentation techniques such as more rotation techniques, cropping, scaling, and potentially adding noise.
