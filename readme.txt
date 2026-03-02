

CNN Digit Recognizer: MNIST Handwritten Classification

This repository contains a complete pipeline for building and training a Convolutional Neural Network (CNN) to recognize handwritten digits. Using the MNIST dataset, the model learns to identify numbers from 0 to 9 with high precision by extracting spatial features through multiple layers of convolutions.

 Project Overview

The goal of this project is to demonstrate how deep learning—specifically CNNs—outperforms traditional machine learning when it comes to image data. Unlike simple flat networks, a CNN looks at "patches" of an image, allowing it to understand shapes, edges, and curves.

 Key Features

* Data Preparation:** The script handles the common "header" issues found in MNIST CSV files, separates labels from pixel data, and normalizes the values for faster convergence.
* Visual Analysis:** Includes a visualization block to display the first few digits of the training set to verify data integrity.
* Layered Architecture:** A balanced mix of Conv2D, MaxPooling, and Dropout layers to ensure the model is both powerful and resistant to overfitting.
* Performance Metrics:** Uses a Confusion Matrix to pinpoint exactly which digits the model finds hardest to distinguish (e.g., mistaking a 4 for a 9).

 Tools and Libraries

* TensorFlow & Keras:** For building and training the deep learning model.
* Pandas & NumPy:** For data structures and matrix mathematics.
* Matplotlib & Seaborn:** For generating clean, readable plots and heatmaps.
* Scikit-Learn:** For splitting the data and generating evaluation reports.

The Model Structure

The network is designed with the following flow:

1. Input: 28 \times 28 grayscale images.
2. Feature Extraction: Two stages of Convolution and Pooling to find patterns.
3. Classification: A Flatten layer followed by a 128-node Dense layer.
4. Regularization: A Dropout layer (20%) to keep the model from "memorizing" the training data.
5. Output:** A 10-node Softmax layer providing the probability for each digit.

How to Get Started

1. Clone the Repo:
`git clone https://github.com/LakshyaGarge/CNN-digit-recognizer.git`
2. Open in Colab:
Upload the `.ipynb` file to Google Colab.
3. Load the Data:
Ensure the `mnist_train_small.csv` and `mnist_test.csv` files are in your `/sample_data/` folder.
4. Run:
Execute the cells in order to train the model and see the results.

