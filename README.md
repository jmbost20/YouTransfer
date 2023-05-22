# YouTransfer: YouTube Transcript Generation with AdversarialVAE

This project was developed in tandem by four students at the University of Wisconsin-Madison to contribute to the topic of text style transfer. The project utilizes Google Colab and Jupyter Notebook to pull transcripts from different YouTube videos and then applies Natural Language Processing (NLP) techniques to generate text using an AdversarialVAE (Variational Autoencoder) model. 

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
  - [Data Collection](#data-collection)
  - [Preprocessing](#preprocessing)
  - [AdversarialVAE Model](#adversarialvae-model)
  - [Results](#results)
- [Contributing](#contributing)

## Introduction

YouTube Transcript Generation with AdversarialVAE is a project that combines the power of NLP and generative models to automatically generate text based on YouTube video content. By leveraging the transcripts available for YouTube videos, this project extracts textual information and employs an AdversarialVAE model to generate realistic and coherent text.

## Packages

This project can be run in Google Colab as it was developed, or it can be ran in a local environment as a .ipynb or converted to .py.

To run this project, you need to have the following dependencies installed:

- pandas
- nltk
- torch
- Python 3.x
- Jupyter Notebook
- TensorFlow
- PyTorch
- Transformers

## Usage

To use with Google Colab: 

Mount your Google Drive by running the code cell containing drive.mount('/content/drive'). This step allows access to the required files and storage for saving the processed data.

Update the channels list variable with the names of the YouTube channels for which you want to clean and prepare the transcript data.

Execute the cells in the notebook one by one. The notebook will perform the following tasks:

1. Load the transcript data for the specified YouTube channels.
2. Perform cleaning and tokenization on the transcript text.
3. Format the transcript data into appropriate inputs for further processing. Save the formatted transcript data, vocabulary mappings, and labels to the specified locations in Google Drive.
4. After executing the notebook, you will have the cleaned and formatted transcript data, vocabulary mappings, and labels saved in the specified locations on your Google Drive.

# Development

The next sections highlight the steps of development this project undertook

## Data Collection

The first step in this project is to collect transcripts from various YouTube videos. The YouTube Data API can be used to retrieve video information, including transcripts, using appropriate API calls. You need to provide API keys and specify the desired YouTube video IDs to fetch the transcripts.

## Preprocessing

Once the transcripts are collected, preprocessing is performed to clean the text data. Preprocessing steps include removing special characters, lowercasing, tokenization, and removing stopwords. These steps help in preparing the data for the AdversarialVAE model.

## AdversarialVAE Model

The AdversarialVAE model is a generative model that combines the principles of variational autoencoders and adversarial training. It consists of an encoder, decoder, and discriminator. The encoder encodes input text into a latent space, the decoder reconstructs the input text from the latent space, and the discriminator tries to distinguish between real and generated text. The model is trained using a combination of reconstruction loss, KL divergence, and adversarial loss.

## Results

The results are best exemplified in the . The project will next undergo updates and iterations to the modelling steps as well as the addition of a UI to enable ease of use for users.

## Contributing

Contributions to this project are welcome. If you have any suggestions, bug fixes, or additional features, feel free to open a pull request. Please ensure that your contributions align with the project's coding style and guidelines.


