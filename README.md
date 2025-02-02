# Leaf-Disease-Detection-Model-using-Deep-Learning
Leaf Disease Detection Model using Deep Learning

# introduction

Agriculture plays a crucial role in the global economy, and plant health is essential for ensuring high crop yields. However, plant diseases can significantly impact agricultural productivity, leading to economic losses and food shortages. Traditional methods of disease detection, such as manual inspection, are time-consuming, labor-intensive, and prone to human error.

To address these challenges, deep learning-based leaf disease detection has emerged as an effective solution. By leveraging convolutional neural networks (CNNs), this approach can automatically identify and classify plant diseases with high accuracy. TensorFlow, an open-source deep learning framework, provides powerful tools for building and training deep neural networks, making it an ideal choice for developing an automated disease detection system.

In this project, a deep learning model is trained on a dataset of healthy and diseased leaf images. The model learns to recognize patterns and features in leaves to classify them into different disease categories.

Key Technologies and Skills
Python
TensorFlow
Convolutional Neural Network (CNN)
Keras
Numpy
Matplotlib

# Data Collection

We acquired the Leaf Disease Image Dataset from Kaggle, a well-known platform for datasets and data science resources. This dataset contains images of potato plant leaves, and Apple plant leaves, carefully categorized into three classes: Early Blight, Late Blight, and Healthy. Each image is meticulously labeled, providing a reliable foundation for training deep learning models in disease detection.
DataSet Link - https://www.kaggle.com/datasets/arjuntejaswi/plant-village

# Preprocessing
In the preprocessing phase, we utilize TensorFlow to read images from the dataset directory. Each image is resized to a standardized 256×256 pixels to ensure consistency across the dataset. Additionally, the processed images are grouped into batches of 32, creating a well-structured dataset optimized for efficient training and analysis

To ensure a thorough evaluation of the model, we divide the dataset into three distinct subsets: training, validation, and testing. This segmentation allows for a structured learning process, where the model is trained on one set, fine-tuned using validation data, and evaluated on unseen test samples. This approach helps minimize overfitting and enhances the model’s ability to generalize effectively to new data.

# Model Building and Training
We design the model architecture using Keras, integrating preprocessing layers for resizing, rescaling, random flipping, and random rotation to enhance data augmentation. The core of the model is a Convolutional Neural Network (CNN), consisting of convolutional layers, pooling layers, and dense layers. These layers are equipped with adjustable filters, units, and activation functions, enabling the model to effectively learn and classify leaf diseases from images.

During model training, we employ the Adam optimizer, sparse_categorical_crossentropy loss function, and accuracy as the evaluation metric to optimize performance. The training process includes validating the model after each epoch to monitor improvements and prevent overfitting. Finally, the model is evaluated on the test dataset, achieving an impressive accuracy of 92.62%, demonstrating its effectiveness in accurately classifying Leaf disease images.


