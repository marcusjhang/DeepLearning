## Setting up your vitual environment

1. pip install virtualenv
2. virtualenv venv
3. source venv/bin/activate
4. which python 
5. python -m pip install jupyter
6. python -m ipykernel install --user --name=venv
7. pip install tensorflow 
8. jupyter notebook

deactivate


## Overfitting and Underfitting
	•	Overfitting occurs when a model learns the training data too well, including its noise and outliers. As a result, the model performs exceptionally well on the training data but poorly on new, unseen data.

Causes:

	1.	Complex Model: Using a model with too many parameters (e.g., a deep neural network with many layers and neurons) relative to the amount of training data can lead to overfitting.
	2.	Insufficient Data: Having a small training dataset makes it easier for the model to memorize the training data rather than learn general patterns.
	3.	Too Many Epochs: Training the model for too many epochs can cause it to learn the noise in the training data.

Symptoms:

	•	High accuracy on the training data but significantly lower accuracy on the validation/test data.
	•	Large gap between training and validation/test performance metrics.

Underfitting

Definition:

	•	Underfitting occurs when a model is too simple to capture the underlying patterns in the data. As a result, it performs poorly on both the training data and the validation/test data.

Causes:

	1.	Simple Model: Using a model that is not complex enough (e.g., a linear model for a problem that requires a more complex representation).
	2.	Insufficient Training: Not training the model for enough epochs.
	3.	High Bias: Strong assumptions about the data that do not hold (e.g., assuming linearity in a non-linear problem).

Symptoms:

	•	Low accuracy on both the training data and the validation/test data.
	•	Small gap between training and validation/test performance metrics, both of which are poor.

## Back Propagation + Loss Calculation
- Back propagation: 
1. input is passed into network
2. loss is calculated using a loss function (mean squared error etc)
3. weights of hidden layers and biases are modified to reduce the loss value