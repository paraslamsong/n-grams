This repository contains an implementation of an N-Gram Language Model. The model supports unigrams (n=1), bigrams (n=2), and trigrams (n=3). It allows for training the model on text data, predicting the next word given a context, and evaluating the model using perplexity.

### Overview

An N-Gram model is a statistical language model that predicts the next word based on the previous n-1 words. In this repository, the model supports:

**Unigram (n=1):** Each word is predicted independently, without considering the context.

**Bigram (n=2):** The model predicts the next word based on the previous word.

**Trigram (n=3):** The model predicts the next word based on the previous two words.

The model uses Add-One (Laplace) smoothing to handle unseen words and calculate probabilities. Additionally, it calculates perplexity, which is used to evaluate how well the model predicts a test dataset.

### Dataset

This process involves the following steps:

**1. Extracting Text from the IsmaelMousa Corpus:** Text is extracted from the IsmaelMousa corpus dataset, which is downloaded from Hugging Face.

**2. Creating Text Files:** For each document in the corpus, a corresponding .txt file is generated and stored in the txt folder.

**3. Creating Train and Validation Text Files:** Created training and validating txt file for the N gram Model.

**4. Tokenization:** The .txt file is used to generate tokens for training n-grams.

To reduce the size of the training data, only the first 100,000 tokens are selected for n-gram model training.
