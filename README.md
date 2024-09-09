# LSTM-Based Chatbot

This project implements a chatbot using a Long Short-Term Memory (LSTM) neural network in PyTorch. The chatbot is designed to process and respond to text inputs, training on a text dataset to learn patterns in conversations.

## Dataset

The project uses a text dataset (AG News) that has been processed and structured into CSV files for training and testing. The data includes columns such as `Class`, `Title`, and `Content`, which are preprocessed to form the `Article` column used for training the model.

### Dataset Structure

The dataset is stored in the following format:
- **Training file**: Contains the text used for training the LSTM model.
- **Test file**: Contains the text used for evaluating the model's performance.

Each file has multiple rows of text data corresponding to different articles.

## Model Architecture

The chatbot uses an LSTM model with the following key features:
1. **Embedding layer**: Converts input text tokens into dense vectors.
2. **LSTM layers**: The core of the model, responsible for learning sequential dependencies in text.
3. **Fully connected output layer**: Generates responses based on the processed sequence data.

The following hyperparameters are used for training:
- **Learning rate**: `1e-4`
- **Number of epochs**: 40
- **Batch size**: 64
- **Maximum input length**: 64 tokens

## Data Preprocessing

Before training, the text data undergoes the following preprocessing steps:
- Tokenization using a SentencePiece model.
- Conversion of text data into numerical sequences suitable for LSTM input.

### Tokenization
A SentencePiece model is generated with a vocabulary size of 20,000 tokens. The model is applied to the dataset, transforming the raw text into token sequences.

## Training

The LSTM model is trained using the following approach:
1. **Load the dataset**: Training and test data are loaded using a custom `Dataset` class.
2. **Preprocess the data**: Text is cleaned and tokenized into sequences.
3. **Train the model**: The LSTM model is trained using the preprocessed text data, with backpropagation and optimization techniques.

## Accuracy and Evaluation

The model’s performance is evaluated based on accuracy over the test data. The custom accuracy function computes the percentage of correct predictions made by the model during testing.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/lstm-chatbot.git
- **Training file**: Contains the text used for training the LSTM model.
- **Test file**: Contains the text used for evaluating the model's performance.

Each file has multiple rows of text data corresponding to different articles.

## Model Architecture

The chatbot uses an LSTM model with the following key features:
1. **Embedding layer**: Converts input text tokens into dense vectors.
2. **LSTM layers**: The core of the model, responsible for learning sequential dependencies in text.
3. **Fully connected output layer**: Generates responses based on the processed sequence data.

The following hyperparameters are used for training:
- **Learning rate**: `1e-4`
- **Number of epochs**: 40
- **Batch size**: 64
- **Maximum input length**: 64 tokens

## Data Preprocessing

Before training, the text data undergoes the following preprocessing steps:
- Tokenization using a SentencePiece model.
- Conversion of text data into numerical sequences suitable for LSTM input.

### Tokenization
A SentencePiece model is generated with a vocabulary size of 20,000 tokens. The model is applied to the dataset, transforming the raw text into token sequences.

## Training

The LSTM model is trained using the following approach:
1. **Load the dataset**: Training and test data are loaded using a custom `Dataset` class.
2. **Preprocess the data**: Text is cleaned and tokenized into sequences.
3. **Train the model**: The LSTM model is trained using the preprocessed text data, with backpropagation and optimization techniques.

## Accuracy and Evaluation

The model’s performance is evaluated based on accuracy over the test data. The custom accuracy function computes the percentage of correct predictions made by the model during testing.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/lstm-chatbot.git

This `README.md` provides a structured overview of your LSTM chatbot project, covering the dataset, model, and training process. Let me know if you'd like to add more details or change anything! &#8203;:contentReference[oaicite:0]{index=0}&#8203;
