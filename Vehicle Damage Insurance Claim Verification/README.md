# Project Overview
This project focuses on building a Convolutional Neural Network (CNN) to classify vehicle damage from images. The model is designed to assist in verifying insurance claims by automatically identifying specific types of damage such as crack, scratch, tire flat, dent, glass shatter, and lamp broken.

# Methodology
The project involved the following steps:  
Dataset Preparation: The provided training set images were mapped to their corresponding damage categories.  
Data Augmentation: An ImageDataGenerator was used to augment the training data with parameters like rescale, rotation_range, width_shift_range, height_shift_range, and zoom_range to prevent overfitting.  
Model Development:  
Base CNN Model: A basic CNN architecture was developed with three Conv2D layers, MaxPooling2D layers, and a final Dropout and Dense layer.  
Regularization: The model was improved by incorporating Batch Normalization and L2 regularization to enhance performance and reduce overfitting.  
Hyperparameter Tuning: Additional parameters like the Adam optimizer learning rate, dropout rate, and number of epochs were tuned to find the optimal configuration for the model.  
Architecture: The final model architecture was a three-layer neural network with a dropout rate of 0.1. The training process utilized the Adam optimization algorithm with a learning rate of 0.01.  

## Key Findings & Results
The best-performing model was the tuned CNN with additional hyperparameters, which achieved a training accuracy of 0.7206 and a validation accuracy of 0.6791.

## Overfitting Analysis
Overfitting was observed in both the model with regularization and the model with hyperparameter tuning, as the training accuracy and loss values were better than the validation values. This was particularly evident in the fluctuations of the validation accuracy.

## Confusion Matrix
The confusion matrix for the final model showed its ability to distinguish between different damage classes. While the model struggled with some classes, it performed better with others, suggesting that more data or advanced techniques might be needed to improve prediction for specific damage types.

# Technologies Used
Python: Core programming language.
Pandas: For data handling and analysis.
Keras/TensorFlow: Used to build, train, and evaluate the CNN models.
ImageDataGenerator: For image data augmentation.
Matplotlib/Seaborn: For plotting accuracy, loss, and confusion matrices.
Scikit-learn: For data splitting and performance metrics.
