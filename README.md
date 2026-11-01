# Customer Churn Prediction

This notebook uses customer account and profile data to predict whether a bank customer will leave (`Exited`). It compares a feed-forward neural network with SimpleRNN and LSTM experiments on structured features.

## Workflow

- Upload `Churn_Modelling.csv` in Google Colab.
- Remove identifier and name fields (`RowNumber`, `CustomerId`, and `Surname`).
- Encode categorical fields and separate the `Exited` target from the input features.
- Split the data into train and test sets and scale numeric features.
- Train an MLP, a SimpleRNN, and an LSTM model; inspect training and validation loss/accuracy curves.
- Evaluate predictions with accuracy, a classification report, and a confusion matrix.

## Dataset

The notebook expects `Churn_Modelling.csv` with an `Exited` column. It is not included in this repository; upload it to the Colab runtime when prompted.

## Run in Google Colab

1. Open `churnmodelling.ipynb` in Google Colab.
2. Upload `Churn_Modelling.csv`.
3. Execute the cells from top to bottom and review the evaluation output.

The neural networks are trained on tabular features, with RNN/LSTM inputs reshaped to one time step. These experiments demonstrate model comparison; they do not represent sequential customer histories. Results depend on the data and runtime.

## Repository contents

- `churnmodelling.ipynb` — data preparation, MLP/RNN/LSTM experiments, and evaluation.
- `README.md` — project overview and usage instructions.

## Author

Gizem Bektaş
