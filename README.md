# Spamurai: Gmail Spam Protection Extension

Spamurai is a Chrome extension designed to enhance Gmail's defense against spam emails. It classifies incoming emails as either spam or non-spam (ham) based on a model trained with a comprehensive dataset of labeled emails. The goal is to help users identify and manage spam emails more effectively.  
[Link to Spamurai Extension](https://spamurai.online/)

## Features

- Classifies emails as spam or non-spam (ham) using advanced machine learning
- Helps improve email organization by filtering spam effectively
- Additional safety checks for Gmail (more details on the website)

## Training the Model

This repository contains the Jupyter notebook used for training the spam classification model for Spamurai. The notebook details the entire process, from data preparation to model evaluation. Here's a brief overview of the steps involved:

### Data Preparation
I use a dataset of labeled emails (around 5,000 emails from Kaggle) to train the model. The data is balanced by downsampling, and preprocessing steps like removing punctuation and stopwords are applied.

You can access the email dataset used for training [here](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset).

### Model Building
A Long Short-Term Memory (LSTM) model is used to classify emails. The model uses an LSTM architecture to classify emails based on the content of the email body. The model is trained using TensorFlow and Keras.

### Evaluation
The model's performance is evaluated using accuracy (you can extend it to other metrics like precision, recall, and F1 score as needed).

### Prediction
The trained model can be used to predict whether a given email is spam or not (you can use this in the extension once integrated with Gmail).

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
