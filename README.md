# Anime-Recommender
Research members: Alejandro Munoz; Chun Ho Wong; Edmund Wong; Yuan Wang; Dong Liu

This code is designed to analyze and process an anime dataset for various purposes. It consists of several tasks such as data preprocessing, normalization, clustering, correlation analysis, K-Nearest Neighbors (KNN) implementation, and Non-negative Matrix Factorization (NMF).

## Data Preprocessing

The code starts with loading the dataset and performing some preprocessing steps:
1. Removing movies from the data by filtering out rows with the 'Type' column equal to 'Movie'.
2. Removing rows with 'Unknown' values.
3. Selecting relevant columns to create a new DataFrame: 'MAL_ID', 'Score', 'Episodes', 'Ranked', 'Popularity', 'Members', 'Favorites'.

## Data Normalization

The selected data is then normalized using the `MinMaxScaler()` from the `sklearn.preprocessing` library.

## Clustering

A K-Means clustering algorithm is applied to the normalized data, and the resulting clusters are visualized using a scatter plot.

## Correlation Analysis

A correlation table is generated using the Pearson correlation method to analyze the relationship between features and the presence of sequels.

## K-Nearest Neighbors (KNN) Implementation

The KNN algorithm is used to classify whether an anime has a sequel or not based on the selected features. The dataset is split into a training set and a test set, and the classifier is trained on the training set. The performance of the classifier is evaluated using a confusion matrix.

## Non-negative Matrix Factorization (NMF)

NMF is applied to the user-anime rating matrix, which is obtained from a separate ratings dataset. The NMF model is used to decompose the ratings matrix into latent factors, and the top anime corresponding to each concept are displayed.

To better understand the code, you may want to run each section separately and analyze the output. This will give you a deeper understanding of the steps involved in the analysis and how the various techniques are applied to the dataset.
