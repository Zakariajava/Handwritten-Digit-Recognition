# Handwritten Digit Recognition

This project implements a deep learning model using TensorFlow and Keras to 
accurately recognize handwritten digits from the MNIST dataset. 
The trained model can then predict digits from user-supplied images.

# Contents

- **`Handwritten-Digit-Recognition.ipynb`**: Jupyter Notebook for training the model, visualizing its performance, and saving it.
- **`predict_digits.py`**: Python script to load the saved model and make predictions on new images.
- **`numbers`**: Directory to store user-provided images for prediction.
- **`handwritten_digit.keras`**: Saved model file containing the trained neural network weights and architecture.
## Installation

Prerequisites: Ensure you have Python 3.6 or later installed.

pip to install the required libraries:
 
```bash
pip install tensorflow opencv-python numpy matplotlib
```

## Training the Model
The model consists of:
- **Input Layer**: Accepts images of size 28x28 pixels.
- **First Hidden Layer**: with 512 units and ReLU activation.
- **Second Hidden Layer**: with 256 units and ReLU activation.
- **Output Layer**: Softmax activation for multi-class classification.

Open Handwritten-Digit-Recognition.ipynb in Jupyter Notebook and run all cells to re-train the model or make your changes on the model and save it as handwritten_digit.keras.

## Making Predictions
To make predictions on new images:
1. Place your images in the numbers/ folder. Ensure that the images are in PNG format and named without the extension (e.g., 0.png).
2. Run the predict_digits.py script. This script will:
 - Load the saved model.
 - Process the images in the numbers/ folder.
 - Display the predictions.
