# Digit_recognizer
MNIST Digit Classification - Convolutional Neural Network (CNN)

# Overview:
This project uses a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset. The model predicts digits (0-9) based on grayscale images of 28x28 pixels.

# Dataset:
The dataset consists of two CSV files:

- train.csv: Contains labeled training data with 784 features (28x28 pixels) and a label column indicating the digit.
- test.csv: Contains 28x28 pixel data for test images (no labels).
  
# Model Description:
The model architecture consists of:

1 Conv2D Layers: Three convolutional layers to extract features from the images.
2 MaxPooling Layers: To downsample the feature maps.
3 Dense Layer: A fully connected layer for classification.
4 Softmax Output Layer: Outputs probabilities for each of the 10 digits (0-9).

# Steps:
1 Data Preprocessing: The pixel values are normalized to the range [0, 1] and reshaped to match the input shape of the CNN (28x28x1).
2 Model Training: The model is trained using the Adam optimizer and categorical crossentropy loss for multi-class classification.
3 Predictions: The trained model predicts the digit labels for the test set.

# Installation
To run the model, make sure you have Python 3.x and the required libraries installed. Use the following command to install dependencies:

!pip install tensorflow numpy pandas matplotlib

#Usage
#Train the Model:

Place the train.csv and test.csv file in the same directory.
Run the script to train the model and evaluate its performance.

Generate Predictions:
-After training, the model will predict labels for the test set (test.csv).
-The results are saved in submission.csv, formatted for Kaggle submission.

# Submission Format
The submission.csv file contains the predictions in the following format:

ImageId	Label
1	3
2	7
3	8
...	...
Model Evaluation
The model is evaluated based on classification accuracy, which is the proportion of correctly predicted labels in the test set.

License
