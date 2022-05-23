# CSE676_DL_Final_Project
Hybrid Deep Learning based Recommender System for the Million song dataset

Data: The Million Song Datatset is available as a snapshot of the EC2 instance and can be downloaded by attaching the snapshot to a custom EC2 instance
Files:
1. Preprocessing: The h5 files were converted to pandas dataframe and saved as csv files. The train_triplet was available as a text file and was converted into a pandas dataframe. Preprocessing includes creating a Collaborative Filtering matrix, created one-hot encoded representation of 'artist_terms', and removing features that are deemed to not contribute to the recommendations
2. autoencoders: Autoencoders for creating latent representaion of the Collaborative Filtering matrix and the sparse one-hot encoded representation of 'artist_terms'
3. Recommender: Final neural network for generating predictions. Combines data from 3 sources, song meta data, collaborative filtering embeddings, 'artist_terms' embeddings. Can be modified based on the features to be used for recommendations
