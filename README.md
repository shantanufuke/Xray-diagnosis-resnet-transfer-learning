# X-Ray Image Diagnosis with ResNet Transfer Learning

## Overview
This project focuses on diagnosing medical conditions from chest X-ray images using deep learning techniques, specifically leveraging transfer learning with ResNet pre-trained on ImageNet. The goal is to classify X-ray images into two categories based on medical diagnoses.

## Dataset
The chest X-ray dataset used in this project is sourced from "Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning." It includes images categorized into 'train', 'val', and 'test' directories, each containing X-ray images resized to the dimensions compatible with ResNet input.

## Dataset Link
You can download the dataset from here https://data.mendeley.com/datasets/rscbjbr9sj/3.

## Data Preprocessing
Image Resizing: Images are resized to match the input size expected by ResNet (224x224 pixels) using bilinear interpolation.
Data Augmentation: Training images are augmented using techniques like rotation, shearing, and horizontal flipping to enhance model generalization.

## Model Architecture
Transfer Learning: The pre-trained ResNet model is loaded and its weights are frozen, except for the last few layers which are fine-tuned.
Custom Layers: Additional layers are added on top of the ResNet base, including flattening, dense, dropout, and output layers tailored for binary classification.

## Conclusion
This project demonstrates the application of transfer learning with ResNet for medical image classification tasks. By leveraging pre-trained models and adapting them to specific medical datasets, we achieve robust classification performance, contributing to improved diagnostic capabilities in healthcare.
