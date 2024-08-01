# Credit Card Fraud Detection
This project aims to build a machine learning model to detect fraudulent credit card transactions. The model is trained using the Credit Card Fraud Detection dataset from Kaggle. A Tkinter-based GUI application is also provided to allow users to input transaction details and get predictions on whether a transaction is fraudulent or legitimate.

# Table of Contents
Installation
Usage
Project Structure
Data
Model
Oversampling
Contributing
License
Installation

To run this project, you'll need Python 3.10+ and several Python libraries. You can install the required libraries using pip:

pip install -r requirements.txt

The requirements.txt file should contain the following dependencies:

pandas
scikit-learn
joblib
tk
imblearn

# Usage
Training the Model
To train the model and save it, run the train_model.py script:

python train_model.py

# Project Structure

credit_card_fraud_detection/
├── data/
│   └── creditcard.csv     # The dataset
├── model/
│   └── model.pkl          # The saved model (after training)
├── app.py                 # The Tkinter application script
├── train_model.py         # The script to train and save the model
├── requirements.txt       # The dependencies
└── README.md              # This README file

# Data
The dataset used for this project is the Credit Card Fraud Detection dataset from Kaggle. It contains transactions made by European cardholders in September 2013. The dataset has the following columns:

# Time
V1 to V28 (anonymized features)

# Amount
Class (target variable: 0 for legitimate, 1 for fraudulent)

# Model
Multiple classifiers are used for this project. The model is trained to classify transactions as fraudulent or legitimate based on the features in the dataset.

# Oversampling
Since the dataset is highly imbalanced, with the majority of transactions being legitimate and a small fraction being fraudulent, we apply oversampling to the minority class (fraudulent transactions) to balance the dataset. This is achieved using the SMOTE (Synthetic Minority Over-sampling Technique) from the imblearn library. This helps the model to better learn and detect fraudulent transactions.

C# ontributing
Contributions are welcome! If you have any ideas or improvements, feel free to open an issue or submit a pull request.

Fork the repository.
Create a new branch: git checkout -b feature/your-feature.
Make your changes and commit them: git commit -m 'Add some feature'.
Push to the branch: git push origin feature/your-feature.
Open a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for details.
