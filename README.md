# SVHN Digit Recognition using CNN
## Objective
The objective of this project is to build a Convolutional Neural Network (CNN) model for digit recognition using the Street View House Numbers (SVHN) dataset. The model aims to achieve high accuracy in classifying images of house numbers into 10 different digit categories (0-9).

## Brief Description
The SVHN dataset contains over 600,000 labeled digits (cropped house number images) obtained from Google Street View images. In this project, we use a subset of the SVHN dataset, available in grayscale format with training, validation, and testing sets.

## Steps Involved:
### Importing Libraries: 
Required libraries include TensorFlow, Keras, NumPy, Matplotlib, Seaborn, and OpenCV for deep learning and image processing.

### Data Preprocessing: 
The dataset is loaded and preprocessed by normalizing the pixel values and converting the labels to categorical format.

### Data Visualization:
Visualizations of the dataset’s class distribution and sample images are plotted using Seaborn and Matplotlib to gain insights.

## Model Building:

#### A Convolutional Neural Network (CNN) is designed with multiple layers:
#### Convolutional layers for feature extraction.
#### Batch Normalization to stabilize and speed up training.
#### Dropout layers to reduce overfitting.
#### Dense layers with softmax activation for final classification.
## Training: 
The model is trained on the training data, with real-time validation on the validation set over 20 epochs. The learning progress is visualized using accuracy and loss plots.

## Model Testing: 
The final model is tested on unseen test data, and performance metrics such as accuracy, precision, recall, and F1-score are calculated.

Performance Visualization: Accuracy and loss for both training and validation are plotted. Predictions on the test data are also visualized alongside the true labels.

## Key Results:
#### Training Accuracy: ~96%
#### Validation Accuracy: ~92%
#### Test Accuracy: ~91%
#### Highest Accuracy Achieved: 96% with the third CNN model with increased convolutional layers and Batch Normalization.

## Dataset
The dataset used in this project is the SVHN Single Digit dataset (grayscale format), which can be downloaded from Kaggle. The dataset contains the following components:

#### X_train, y_train: Training data and labels.
#### X_val, y_val: Validation data and labels.
#### X_test, y_test: Test data and labels.
## Conclusion
The CNN model successfully classifies digits from the SVHN dataset with an accuracy of 96%. Further tuning and model optimization can improve performance, but the results demonstrate the effectiveness of convolutional networks for image-based digit classification. By incorporating additional techniques like Batch Normalization and Dropout, we minimized overfitting and improved generalization to unseen data.
