# Customer Churn Prediction

This code implements a customer churn prediction model using a neural network built with TensorFlow.

## Data
The data used for this project is taken from the Kaggle dataset "Telco Customer Churn". It includes information about customers such as their contract type, internet service, monthly charges, tenure, and whether or not they have churned (i.e. left the company).

## Data Preprocessing
The following data preprocessing steps were applied to the dataset:
- Removing the customerID column as it is not relevant to the prediction task.
- Converting the TotalCharges column to a numeric type.
- Removing rows where TotalCharges is empty.
- Converting the Churn column from 'Yes'/'No' to 1/0.
- Converting other columns with 'Yes'/'No' values to 1/0.
- One-hot encoding the Contract, InternetService, and PaymentMethod columns.
- Scaling the tenure, MonthlyCharges, and TotalCharges columns using MinMaxScaler.

## Neural Network
The neural network used for this project has an input layer, two hidden layers with 26 and 15 neurons respectively, and an output layer with a single neuron. The activation function used for the hidden layers is ReLU, and the output layer uses the sigmoid function. The model is trained using the binary cross-entropy loss function and the Adam optimizer.

## Conclusion
This project demonstrates how a neural network can be used to predict customer churn. By preprocessing the data and training a neural network, we can make predictions about which customers are likely to churn, and take steps to retain them before they leave.
