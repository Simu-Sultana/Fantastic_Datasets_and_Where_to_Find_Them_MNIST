# MNIST Handwritten Digit Recognition

This project focuses on handwritten digit classification using the MNIST dataset. It demonstrates both classical machine learning (KNN) and deep learning (CNN) approaches for image classification.

The project follows a complete workflow: understanding the dataset, preprocessing the data, applying a baseline model, building a deep learning model, and visualizing the results.

---

## Dataset

The MNIST dataset (Modified National Institute of Standards and Technology) is one of the most widely used datasets in machine learning and computer vision. It is often referred to as the "Hello World" dataset for deep learning. :contentReference[oaicite:0]{index=0}

- 70,000 grayscale images
- Image size: 28 × 28 pixels
- 10 classes (digits 0–9)
- 60,000 training samples
- 10,000 test samples

Each image consists of 784 pixel values (28 × 28), where pixel intensities range from 0 (black) to 255 (white). :contentReference[oaicite:1]{index=1}

Dataset link:
https://www.kaggle.com/datasets/hojjatk/mnist-dataset

The dataset is not included in this repository. Please download it from the link above if needed.

---

## Project Structure

```text
Fantastic_Datasets_and_Where_to_Find_Them_MNIST/
│
├── notebooks/
│   ├── 01_pixel_value_generation.ipynb
│   ├── 02_knn_mnist_classification.ipynb
│   ├── 03_cnn_model_building.ipynb
│   └── 04_plotting_results.ipynb
│
├── data/
│   └── README.md
│
├── video/
│   └── video_link.txt
│
├── results/
│
├── requirements.txt
└── README.md
```

## Notebooks Overview

### 1. Pixel Value Generation

This notebook explores how MNIST images are represented numerically. It demonstrates how images are stored as pixel matrices and how they can be visualized.

### 2. KNN Classification

This notebook implements the K-Nearest Neighbors (KNN) algorithm as a baseline model for handwritten digit classification. It includes model training, prediction, confusion matrix, and classification report.

### 3. CNN Model Building

This notebook builds a Convolutional Neural Network (CNN) for digit classification.

The model:
- Reshapes images into 28×28×1 format
- Normalizes pixel values to the range [0, 1]
- Uses convolutional layers for feature extraction
- Applies max pooling for dimensionality reduction
- Uses dropout to prevent overfitting
- Outputs predictions using a softmax layer

The CNN is trained for 5 epochs with a batch size of 64 and achieves over 99% accuracy.

### 4. Results Visualization

This notebook visualizes model performance using:
- Accuracy plots
- Loss plots
- Model comparison between KNN and CNN

---

## Methodology

### Data Preprocessing

- Images are reshaped into 4D tensors (28 × 28 × 1)
- Pixel values are normalized to the range [0, 1]
- Labels are converted into one-hot encoded vectors :contentReference[oaicite:3]{index=3}

### KNN (Baseline Model)

KNN is used as a classical machine learning approach. It classifies digits based on similarity between feature vectors.

### CNN (Main Model)

The CNN model uses:
- Convolutional layers (feature extraction)
- Pooling layers (dimensionality reduction)
- Dropout (regularization)
- Dense softmax layer (classification)

CNN performs significantly better than KNN because it can learn spatial patterns in image data.

---

## Results

- KNN provides a strong baseline performance
- CNN achieves higher accuracy (>99%)
- CNN generalizes better for image classification tasks

---

## Video Explanation

A complete explanation of the project is available here:

https://www.youtube.com/watch?v=SrT6QkQUH4Q

---

## How to Run

Install dependencies:

pip install -r requirements.txt

Start Jupyter Notebook:

jupyter notebook

Run notebooks in order:

1. 01_pixel_value_generation.ipynb
2. 02_knn_mnist_classification.ipynb
3. 03_cnn_model_building.ipynb
4. 04_plotting_results.ipynb

---

## Requirements

- numpy
- pandas
- matplotlib
- scikit-learn
- tensorflow
- keras
- jupyter

---

## Conclusion

The MNIST dataset remains a fundamental benchmark for machine learning. Despite its simplicity, it is highly effective for understanding core concepts in image classification and deep learning. :contentReference[oaicite:4]{index=4}

---

## Author

Simu Sultana