# Customer Churn Prediction

This Google Colab notebook predicts whether a bank customer will leave (`Exited`) using account and profile attributes. It compares a feed-forward neural network with SimpleRNN and LSTM experiments on structured features.

## Workflow

- Load `Churn_Modelling.csv`.
- Remove identifier and name fields (`RowNumber`, `CustomerId`, and `Surname`).
- Encode categorical features and separate the `Exited` target.
- Split the data into training and test sets and scale numeric features.
- Train an MLP, SimpleRNN, and LSTM; review loss and accuracy curves.
- Evaluate predictions with accuracy, a classification report, and a confusion matrix.

## Dataset and access

The notebook expects `Churn_Modelling.csv` with an `Exited` column. The Kaggle [Churn Modelling competition](https://www.kaggle.com/competitions/churn-modelling/data) lists the CSV as **Subject to Competition Rules**. A Kaggle community copy currently shows its license as **Unknown**. Because redistribution rights are not clear, the dataset is not bundled in this repository.

Obtain the data only from a source whose terms you have reviewed and are permitted to use. This project does not accept competition rules on your behalf. Upload your authorized copy to Colab when prompted.

## Run in Google Colab

1. Open `churnmodelling.ipynb` in Google Colab.
2. Upload your authorized `Churn_Modelling.csv` copy.
3. Execute the cells from top to bottom and review the evaluation output.

The neural networks use tabular features, with RNN/LSTM inputs reshaped to one time step. These experiments demonstrate model comparison; they do not represent sequential customer histories. Results depend on the data and runtime.

## Repository contents

- `churnmodelling.ipynb` — data preparation, MLP/RNN/LSTM experiments, and evaluation.
- `README.md` — project overview, data access notes, and usage instructions.

## Author

Gizem Bektaş
