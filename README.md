
This repository contains code for building a predictive model to estimate Blood Alcohol Concentration (BAC) levels based on various factors such as drink consumption, biometric data, and demographic information. The model utilizes Long Short-Term Memory (LSTM) neural networks, a type of recurrent neural network (RNN), implemented using TensorFlow and scikit-learn libraries in Python.

The dataset used in this project is stored in the file `newoutput1.csv`. This dataset contains information about individuals' drink consumption habits, biometric data (height, weight), demographic information (age, sex, ethnicity), and related factors. Before building the model, the dataset is preprocessed to handle missing values and encode categorical variables.

The predictive model is built using a sequential LSTM neural network architecture. LSTM networks are chosen for their ability to capture temporal dependencies in sequential data, making them suitable for time-series prediction tasks like BAC estimation. The model architecture consists of three LSTM layers with dropout regularization to prevent overfitting, followed by dense layers for regression prediction. The model is compiled using the Adam optimizer and Mean Squared Error (MSE) loss function.

The dataset is split into training, validation, and test sets. The model is trained on the training set and validated on the validation set to monitor its performance and prevent overfitting. Training hyperparameters such as batch size and number of epochs are specified for the training process. Once trained, the model is evaluated on the test set to assess its predictive accuracy.
The performance of the model is evaluated using Mean Squared Error (MSE) metric, which measures the average squared difference between the actual and predicted BAC values on the test set. A lower MSE indicates better predictive performance of the model.

