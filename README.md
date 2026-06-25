# MNIST Handwritten Digit Classification using Perceptron, ANN, and CNN

## Project Overview

This project focuses on the classification of handwritten digits from the MNIST dataset using three different machine learning and deep learning models:

- Perceptron (Baseline Model)
- Artificial Neural Network (ANN)
- Convolutional Neural Network (CNN)

The primary objective is to compare the performance of these models and demonstrate how deep learning techniques improve image classification accuracy.

---

## Dataset

The project uses the MNIST Handwritten Digit Dataset containing grayscale images of handwritten digits from 0 to 9.

### Dataset Characteristics

- Total Features: 784 (28 × 28 pixels)
- Classes: 10 (Digits 0–9)
- Image Size: 28 × 28 pixels
- Task: Multi-class Classification

---

## Project Workflow

### 1. Data Preprocessing

- Loaded and explored the dataset
- Separated features and target labels
- Normalized pixel values
- Performed train-test split
- Reshaped data for CNN architecture

---

### 2. Perceptron Model

#### Techniques Used

- Perceptron Classifier
- RandomizedSearchCV for hyperparameter tuning

#### Performance

- Accuracy: ~86%

#### Limitations

- Linear classifier
- Struggles with complex image patterns
- Higher misclassification rate

---

### 3. Artificial Neural Network (ANN)

#### Architecture

- Dense Layers
- ReLU Activation
- Dropout Layers
- Adam Optimizer

#### Performance

- Accuracy: ~97–98%

#### Advantages

- Learns non-linear relationships
- Significant improvement over Perceptron

---

### 4. Convolutional Neural Network (CNN)

#### Architecture

```text
Conv2D
↓
MaxPooling2D
↓
Conv2D
↓
Flatten
↓
Dense
↓
Dropout
↓
Output Layer
```

#### Performance

- Accuracy: ~98–99%

#### Advantages

- Automatic feature extraction
- Learns spatial relationships
- Lowest error rate
- Best overall performance

---

## Model Comparison

| Metric | Perceptron | ANN | CNN |
|----------|----------|----------|----------|
| Accuracy | ~86% | ~97–98% | ~98–99% |
| Precision | Moderate | High | Highest |
| Recall | Moderate | High | Highest |
| F1-Score | Moderate | High | Highest |
| Error Rate | High | Low | Lowest |
| Complexity | Low | Medium | High |

---

## Evaluation Metrics

The following evaluation techniques were used:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix
- Error Rate Analysis
- Misclassification Analysis

---

## Visualizations

The project includes:

- Accuracy Comparison Graph
- Error Rate Comparison Graph
- Precision, Recall, and F1-Score Comparison
- Confusion Matrix Heatmaps
- Correct vs Incorrect Prediction Analysis
- Misclassified Sample Visualization
- CNN Error Analysis

---

## Key Findings

### Perceptron

- Fast and simple baseline model
- Limited by linear decision boundaries
- Lowest performance among all models

### ANN

- Significant improvement over Perceptron
- Successfully learns non-linear patterns
- High classification accuracy

### CNN

- Best performing model
- Achieves highest accuracy and F1-score
- Produces the fewest misclassifications
- Most suitable for image classification tasks

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## Project Structure

```text
MNIST-Project/
│
├── perceptron/
│   ├── perceptron.ipynb
│   └── perceptron_model.pkl
│
├── ann/
│   ├── ann.ipynb
│   └── ann_model.h5
│
├── cnn/
│   ├── cnn.ipynb
│   └── cnn_model.h5
│
├── comparison/
│   └── model_comparison.ipynb
│
├── README.md

```

---

## Conclusion

This project demonstrates the evolution of image classification performance from a simple linear Perceptron to advanced deep learning architectures. While the Perceptron provides a useful baseline, ANN substantially improves performance through non-linear learning. The CNN achieves the best results by effectively extracting spatial features from handwritten digit images, making it the most effective model for MNIST digit classification.

---

## Author

**Nikhil Garg**

Machine Learning & Deep Learning Project – MNIST Digit Classification and Model Comparison.
