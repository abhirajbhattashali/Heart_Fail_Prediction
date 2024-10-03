# Heart Failure Prediction Model

This repository contains a machine learning model developed to predict heart failure events based on clinical records data.

## Dataset

The model is trained on the [Heart Failure Clinical Records Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records). This dataset contains various clinical features that may contribute to heart failure, such as age, ejection fraction, serum creatinine, and others.

## Model Architecture

The model is a neural network built using TensorFlow and Keras. It consists of:

- Input layer
- Hidden layer with 24 neurons and ReLU activation function
- Output layer with 2 neurons (for predicting the presence or absence of heart failure) and softmax activation function
- Here is the model architecture from the script:

```python
# Design the model
model = Sequential()
# Add the input layer
model.add(InputLayer(input_shape=(x_train.shape[1],)))
# Add a hidden layer
model.add(Dense(24, activation='relu'))
# Add an output layer 
model.add(Dense(2, activation='softmax'))
```

## Training

The model was trained using the Adam optimizer and sparse categorical crossentropy loss function. It was evaluated using accuracy and a confusion matrix.


## Evaluation

The model achieved a reasonable accuracy on the test set. A confusion matrix and deviation plot provide further insights into the model's performance.

## Contributing

Contributions are welcome! If you want to improve the model or add new features, feel free to open a pull request.

