# Unsupervised Clustering of Frequently Asked Questions

This project demonstrates an unsupervised approach to organizing and retrieving Frequently Asked Questions (FAQs) using sentence embeddings, KMeans, DBSCAN, and HDBSCAN clustering.

## Overview

The project utilizes the SentenceTransformer model (`all-MiniLM-L6-v2`) to generate dense vector representations of FAQ text.  These embeddings are then clustered using KMeans, DBSCAN, and HDBSCAN.  The optimal number of clusters for KMeans is determined using the Elbow Method and Silhouette Score.  DBSCAN and HDBSCAN are used to identify clusters of varying shapes and densities.  The code includes functions for classifying new questions and retrieving similar questions from the clustered data.

## Data

The project uses a JSON file (`questions.json`) as input.  The JSON file should contain a list of dictionaries, where each dictionary represents an FAQ. Each dictionary should include a `question_text` field.

Adding a new line
- This project is using LLMS for clusteting

## Dependencies

*   transformers
*   sentence-transformers
*   scikit-learn
*   pandas
*   umap-learn
*   hdbscan
*   matplotlib

## Usage

1.  **Installation:** Install the required dependencies using pip:
