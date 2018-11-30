# Recommender Systems

## Movie/TV show Recommender System
Recommender systems are one of the most important applications in data scinece and machine learning.
The repsitory focuses on analyzing MovieLens 1M data for rating prediction and Myanimelist dataset for analyzing
Japanese Animation preferences in large internet community myanimelist. The datasets were from official GroupLens website
and MAL Kaggle dataset containing over 30M user ratings and 14K different shows. Feel free to go into either directory to view both data processing and feature engineering process. Please view colab links for full examples

### movieRec

The Movie directory focuses on analyzing user/movie data to use a hybrid DNN recommendation engine that takes in both user, movie, and rating embeddings for user ratings prediciton. Synthetic features and dimensionality reduction techniques such as PCA were applied to tackle data sparcity issues. Keras models were used for ratings prediction. For similar attempt on using google's wide-and-deep DNN architecture, please check **wide-and-deep-recommender** repository for tensorflow application built for training on GCP's cloud ML engine.

#### Colab links
Hybrid-Movie-Recommender-Data-Processing: 

https://drive.google.com/open?id=1XC0z4G2TKftLC8Ia4o3wdFCf82nvCw4_

Hybrid-Model: https://drive.google.com/open?id=1E8uxPq6S0Wj_vBcpW9jiMY7rBiiAJYEk

### aniRec

The Anime directory focuses on analyzing features of both TV shows and users in-depth. The dataset contains over 20 features for each TV show and user making it a much difficult problem to tackle compared to MovieLens data which is known to have very tidy data. Some of the additonal data were crawled from the internet using a custom Java crawler and also a Python Scrapy spider. These projects can be found in **Recommendation-Engine-Data-Extractor-Java** or **Recommendation-Engine-Data-Extractor-Python** repositories. The EDA notebooks focus on cleaning messy data and adding synthetic features for better recommendations. Regarding the acutal recommendation models, the **content-based-recommendation** notebook focuses on using different similarity matrix for top-N recommendations given a certain show. The **autoencoder** notebook takes pure ratings matrix with Pytorch to build a custom autoencoder for predicting user ratings. In the future, custom SVD++ and Hybrid model with RBM are planning to be added.

#### Colab links
autoencoder_recommendation: https://drive.google.com/open?id=1ICnoJo44j5IiS_hInmcmdTYHx8rJDhFn

content_based_recommendation: https://drive.google.com/open?id=1foGGdyvKeu24aEobRtcbfj4f8oZZ2uoX

users_EDA: https://drive.google.com/open?id=1FPV3twfDU9OF9C7q5M5tvrEnnIz5Cc6X

animes_EDA: https://drive.google.com/open?id=1hOqK3tOYMClZPENX21CiC4aWdVvD3F7g
