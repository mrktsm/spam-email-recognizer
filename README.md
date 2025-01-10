# Spamurai: Gmail Spam Protection Extension

**Spamurai** is a Chrome extension designed to enhance Gmail's defense against spam emails. It classifies incoming emails as either spam or non-spam (ham) based on a model trained with a dataset of SMS messages. The goal is to help users identify and manage spam emails more effectively.

[Link to Spamurai Extension](https://link-to-spamurai-extension.com)

## Features
- Classifies emails as spam or non-spam (ham).
- Helps improve email organization by filtering spam effectively.
- Additional safety checks for Gmail (more details on the website).

## Training the Model
This repository contains the Jupyter notebook used for training the spam classification model for [**Spamurai**](https://spamurai.online/). The notebook details the entire process, from data preparation to model evaluation. Here’s a brief overview of the steps involved:

1. **Data Preparation**: We use a Kaggle dataset of SMS messages to train the model. The data is balanced by downsampling, and unnecessary elements like stopwords and punctuations are removed.
2. **Model Building**: A Long Short-Term Memory (LSTM) model is used to classify emails. The model is trained using TensorFlow and Keras.
3. **Evaluation**: The model's performance is evaluated using accuracy and loss metrics.
4. **Prediction**: The model is capable of predicting whether a new email is spam or not.

You can access the dataset used for training [here]([https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset](https://www.kaggle.com/datasets/meruvulikith/190k-spam-ham-email-dataset-for-classification)).

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
Once the model is trained, it can be integrated into your own system to classify incoming emails, marking them as spam or non-spam based on the classification results.

For more information, visit our website: [Spamurai Website](https://spamurai.online/).

## License
Distributed under the Apache License 2.0. See `LICENSE` for more information.
