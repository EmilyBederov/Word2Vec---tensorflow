# Applied-ML Project: Skip-Gram Model Implementation

## Project Overview
This project implements a Skip-Gram model for learning word embeddings using a dataset of hotel reviews. The model is trained to predict context words from a target word, enabling it to capture the relationships between words. The implementation is optimized for handling large datasets, generating meaningful word embeddings through an efficient and scalable approach.

The project is organized in a Jupyter notebook and includes functions for data preprocessing, vocabulary creation, training data generation (positive and negative samples), model training, and embedding visualization.

## Dataset
The dataset used in this project comprises 230,339 rows of hotel reviews. Raw text is processed to remove both frequent and rare words, refining the vocabulary size. The final vocabulary contains approximately 23,000 words, providing a balanced representation of commonly used terms.

## Key Components

### Data Preprocessing
- **Cleaning and Tokenizing**: Prepares the text data for analysis.
- **Vocabulary Creation**: Builds a vocabulary from the dataset.
- **Subsampling and Filtering**: Subsamples frequent words and removes rare ones based on a set frequency threshold to optimize memory and efficiency.

### Training Data Generation
- **Positive and Negative Pairs**: Creates word pairs using a sliding context window.
- **Negative Sampling**: Implements an efficient negative sampling strategy, generating training data without memory overload.

### Model Architecture
- **Skip-Gram Model**: Implemented using TensorFlow and Keras, this model accepts target and context words as input and trains with negative sampling.

### Word Embeddings
- **Embeddings**: After training, the model produces embeddings for each word, which are useful for tasks such as word similarity and clustering.

### Visualization
- **Dimensionality Reduction**: Techniques such as PCA and t-SNE are applied to visualize word embeddings and explore word relationships within the embedding space.

---

This project showcases a complete pipeline for building and evaluating a Skip-Gram model, from data preprocessing to embedding visualization, providing valuable tools for exploring semantic word relationships.
