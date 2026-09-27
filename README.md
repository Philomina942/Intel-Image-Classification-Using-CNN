
# Intel Image Classification Using CNN

## Project Overview

This project focuses on building a Convolutional Neural Network (CNN) model to classify natural scene images into six different categories using the Intel Image Classification dataset.

The model is developed using TensorFlow and Keras in Google Colab. It uses image preprocessing, data augmentation, and CNN layers to learn visual features and classify images.

## Objectives

- Build a CNN model for multi-class image classification.
- Classify images into six natural scene categories.
- Apply image normalization and data augmentation.
- Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.

## Dataset

**Dataset:** Intel Image Classification

**Source:** [Kaggle - Intel Image Classification](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)

The dataset contains images belonging to six classes:

1. Buildings
2. Forest
3. Glacier
4. Mountain
5. Sea
6. Street

The dataset is organized into training, testing, and prediction image folders.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Model Architecture

The CNN model consists of:

- Input layer: 150 × 150 RGB images
- Data augmentation: Random flip, rotation, zoom, and translation
- Four convolutional layers with 32, 64, 128, and 256 filters
- Max pooling layers
- Global Average Pooling layer
- Fully connected dense layer with 128 neurons
- Dropout layer with a rate of 0.5
- Softmax output layer with six classes

The model uses the Adam optimizer and sparse categorical cross-entropy loss function.

## Model Training

The training dataset was divided into:

- 80% training data
- 20% validation data

The model was trained for up to 20 epochs using early stopping and model checkpointing to help reduce overfitting and save the best-performing model.

## Results

The model was evaluated on 3,000 independent test images.

| Metric | Result |
|---|---:|
| Test Accuracy | 82% |
| Macro F1-score | 0.83 |
| Weighted F1-score | 0.82 |

### Class-wise Performance

| Class | Precision | Recall | F1-score |
|---|---:|---:|---:|
| Buildings | 0.72 | 0.84 | 0.78 |
| Forest | 0.98 | 0.93 | 0.95 |
| Glacier | 0.81 | 0.74 | 0.78 |
| Mountain | 0.82 | 0.73 | 0.77 |
| Sea | 0.81 | 0.86 | 0.83 |
| Street | 0.83 | 0.87 | 0.85 |

Forest images achieved the highest F1-score, while mountain images had the lowest recall.

## How to Run

1. Download or clone this repository.
2. Open the notebook `Intel_CNN_Assignment_Final_Results.ipynb` in Google Colab.
3. Download the dataset from Kaggle using the dataset link above.
4. Upload the dataset ZIP file to your Colab session.
5. Ensure the ZIP file is named `archive.zip`, or update the dataset path in the notebook.
6. Enable GPU acceleration in Colab.
7. Run the notebook cells sequentially.

## Project Structure

```text
Intel-CNN-Image-Classification/
│
├── Intel_CNN_Assignment_Final_Results.ipynb
├── README.md
└── best_cnn_model.keras  (optional, trained model)
```

## Conclusion

This project demonstrates the application of Convolutional Neural Networks to natural scene image classification. The model achieved 82% test accuracy across six categories.

The results show that CNNs can learn meaningful image features and classify different natural scenes. Future improvements could include transfer learning, hyperparameter tuning, and experimentation with different CNN architectures.

## Author

**Tania Philomina**

MCA Student | Machine Learning and Deep Learning

---

*Academic project: Building a CNN Model for Image Classification.*
