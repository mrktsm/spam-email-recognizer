## Spamurai: Gmail Spam Protection Extension Powered by This Neural Network

The Spamurai Gmail spam protection extension is powered by the neural network developed in this repository. By classifying incoming emails as spam or non-spam (ham), this AI-driven solution enhances Gmail's defense against unwanted emails, helping users manage their inbox effectively.

[Explore Spamurai](https://spamurai.online/)

## Features

- Classifies emails as spam or non-spam (ham) using advanced machine learning
- Helps improve email organization by filtering spam effectively
- Additional safety checks for Gmail (more details on the website)

## Training the Model

This repository contains the Jupyter notebook used for training the spam classification model. The notebook details the entire process, from data preparation to model evaluation. Here's a brief overview of the steps involved:

### Data Preparation
I use a dataset of labeled emails (around 200,000 emails from Kaggle) to train the model. The data is balanced by downsampling, and preprocessing steps like removing punctuation and stopwords are applied.

You can access the email dataset used for training [here](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset).

### Model Building
A Long Short-Term Memory (LSTM) model is used to classify emails. The model uses an LSTM architecture to classify emails based on the content of the email body. The model is trained using TensorFlow and Keras.

### Evaluation
The model's performance is evaluated using accuracy (you can extend it to other metrics like precision, recall, and F1 score as needed).

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/your-username/spamurai.git
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the Jupyter notebook to train the model and evaluate its performance.

## Usage
Now you can integrate the model into your own project. Once the model is trained, you can use it to classify incoming emails, marking them as spam or non-spam based on the classification results.

## License
Distributed under the Apache-2.0 License. See `LICENSE` for more information.
