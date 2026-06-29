# Handwritten Digit Recognition using Neural Networks (MNIST)

This project implements Artificial Neural Network to classify handwritten digits from the MNIST dataset. The model is trained to recognize digits from 0 to 9 using deep learning techniques and achieves an accuracy of approximately 97.369% on the test dataset.

The main objective of this project is to:

* Understand the fundamentals of Neural Networks.
* Build and train a feedforward neural network using TensorFlow and Keras.
* Classify handwritten digit images from the MNIST dataset.
* Evaluate the performance of the model using accuracy and loss metrics.

Dataset: MNIST Handwritten Digits Dataset

* Training Images: 60,000
* Testing Images: 10,000
* Image Size: 28 × 28 pixels
* Number of Classes: 10 (digits 0-9)

Dataset Link:
https://www.kaggle.com/datasets/hojjatk/mnist-dataset

python version used is 3.11(.venv) Python(3.11.9) #since tensorflow is not supported on other ver

#  Model Architecture


Input Image (28×28)
        ↓
Flatten Layer (784 neurons)
        ↓
Dense Layer (128 neurons, ReLU)
        ↓
Dense Layer (64 neurons, ReLU)
        ↓
Output Layer (10 neurons, Softmax)
        ↓
Predicted Digit


# Results

* Test Accuracy: 97.37%
* Test Loss: Generated during model evaluation.

The model successfully learns patterns from handwritten digits and performs highly accurate classification.

The project includes:

* Training Accuracy vs Validation Accuracy Graph
* Training Loss vs Validation Loss Graph
* Sample Predictions on Test Images


# Conclusion
A feedforward neural network was developed to classify handwritten digits from the MNIST dataset. After preprocessing and training for 10 epochs using the Adam optimizer and categorical cross-entropy loss, the model achieved an accuracy of approximately 97.4% on the test dataset, demonstrating the effectiveness of neural networks for image classification.
