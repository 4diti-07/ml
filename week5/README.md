# CNN Image Classification using TensorFlow & Keras

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify handwritten digits from the MNIST dataset. The model learns patterns from thousands of labeled images and predicts the correct digit (0–9) for unseen images.

So i have made this project with the assistance of AI, and understood the difference btwn tensorflow and pytorch.

The objective of this project is to:

* Understand the working of Convolutional Neural Networks (CNNs).
* Build and train a CNN using TensorFlow and Keras.
* Classify handwritten digits from the MNIST dataset.
* Evaluate the model's performance on unseen test data.
* Visualize the model's training performance and predictions.

Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Jupyter Notebook / VS Code

The project uses the MNIST Handwritten Digits Dataset, which contains grayscale images of handwritten digits.


# Why we use TensorFlow?
TensorFlow is an open-source machine learning framework developed by Google. It provides the computational engine required to build, train, and evaluate deep learning models.

TensorFlow is responsible for:

* Performing mathematical computations.
* Training the neural network.
* Updating model parameters during backpropagation.
* Optimizing the model using the selected optimizer.
* Running efficiently on CPUs and GPUs.

# Why we use Keras?
Keras is TensorFlow's high-level API that simplifies the process of building neural networks.

Instead of manually implementing every mathematical operation, Keras provides pre-built layers and training functions.

Using Keras allows us to:

* Build models with fewer lines of code.
* Create readable and modular neural network architectures.
* Train models using simple methods such as `model.fit()`.
* Evaluate models easily using `model.evaluate()`.

# Why TensorFlow and Keras Together?
TensorFlow acts as the backend computational engine, while Keras provides a simple interface for designing and training neural networks.

# CNN Architecture

The implemented CNN consists of the following layers:

```
Input (28 × 28 × 1)
        │
        ▼
Conv2D (32 filters, 3×3)
        │
        ▼
ReLU Activation
        │
        ▼
MaxPooling2D (2×2)
        │
        ▼
Conv2D (64 filters, 3×3)
        │
        ▼
ReLU Activation
        │
        ▼
MaxPooling2D (2×2)
        │
        ▼
Flatten
        │
        ▼
Dense (64 neurons)
        │
        ▼
Dense (10 neurons, Softmax)
```

# TensorFlow/Keras vs PyTorch

| TensorFlow & Keras             | PyTorch              |
| ------------------------------ | -------------------- |
| High-level API                 | Lower-level API      |
| Less code                      | More code            |
| Built-in `model.fit()`         | Custom training loop |
| Easier for beginners           | Greater flexibility  |
| Suitable for rapid development | Popular in research  |

Although both frameworks implement the same deep learning concepts, TensorFlow with Keras offers a simpler and more concise approach for beginners.

# Conclusion
This project demonstrates how a Convolutional Neural Network can accurately classify handwritten digits using TensorFlow and Keras. By combining convolution, activation, pooling, flattening, and dense layers, the model learns meaningful image features and achieves high classification accuracy on the MNIST dataset. The project also highlights the advantages of TensorFlow and Keras for building deep learning models in a simple, readable, and efficient manner.

# Results
The trained CNN achieves approximately **99% test accuracy** on the MNIST dataset, demonstrating the effectiveness of CNNs for handwritten digit recognition.

The notebook also includes:

* Training Accuracy vs Validation Accuracy
* Training Loss vs Validation Loss
* Sample Predictions

# References

* TensorFlow Official Documentation: https://www.tensorflow.org/tutorials
* Keras Official Documentation: https://keras.io/
* TensorFlow MNIST Dataset Documentation: https://www.tensorflow.org/api_docs/python/tf/keras/datasets/mnist
* TensorFlow Conv2D Documentation: https://www.tensorflow.org/api_docs/python/tf/keras/layers/Conv2D
* TensorFlow MaxPooling2D Documentation: https://www.tensorflow.org/api_docs/python/tf/keras/layers/MaxPooling2D
