# Song Genre Clustering and Recommendation System

## Project Overview
This project explores and implements clustering techniques to group songs by their audio features, creating a recommendation system based on the natural grouping of genres. Using Spotify's dataset, we apply both unsupervised and supervised learning methods to identify clusters, predict genres, and make song recommendations based on genre similarities.

## Dataset
The data used in this project comes from the [Spotify Tracks Dataset on Kaggle](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset). This dataset provides a rich array of audio features for each track, enabling a comprehensive analysis and clustering of songs based on musical characteristics.

### Column Descriptions
- **track_id**: The unique Spotify ID for each track.
- **artists**: Names of artists who performed the track, separated by a semicolon if multiple.
- **album_name**: Name of the album in which the track appears.
- **track_name**: Name of the track.
- **popularity**: Popularity score from 0 to 100, calculated based on the number and recency of plays.
- **duration_ms**: Length of the track in milliseconds.
- **explicit**: Indicates if the track has explicit lyrics (`true` or `false`).
- **danceability**: Danceability score from 0.0 to 1.0, indicating suitability for dancing.
- **energy**: Measure of intensity from 0.0 to 1.0.
- **key**: Musical key of the track, represented as an integer (0 = C, 1 = C♯/D♭, etc.).
- **loudness**: Overall loudness in decibels (dB).
- **mode**: Modality of the track; 1 represents major, 0 represents minor.
- **speechiness**: Measure from 0.0 to 1.0 indicating presence of spoken words.
- **acousticness**: Confidence from 0.0 to 1.0 that the track is acoustic.
- **instrumentalness**: Likelihood from 0.0 to 1.0 that the track contains no vocals.
- **liveness**: Probability from 0.0 to 1.0 that the track was performed live.
- **valence**: Measure from 0.0 to 1.0 of the track’s musical positiveness.
- **tempo**: Track tempo in beats per minute (BPM).
- **time_signature**: Time signature of the track, ranging from 3 to 7.
- **track_genre**: Genre label for the track.

## Methods
This project employs the following data science methods:

1. **General Clustering Algorithms**: Initial clustering of songs based on audio features using algorithms like k-means and DBSCAN to uncover natural groupings.

2. **Graph Clustering Algorithms**: Using graph clustering techniques such as Spectral Clustering or Louvain Algorithm, we analyze connections between songs based on feature similarity, revealing nuanced communities of tracks.

3. **Supervised Learning**: We apply supervised learning, such as Random Forest or SVM, to predict genres based on known labels in the dataset, validating and refining the clustering results.

4. **Recommendation System**: Based on clusters and genre predictions, we design a recommendation system that suggests songs within or across clusters based on similarity measures.

## Project Goals
- Group songs by genre and other musical characteristics.
- Implement a recommendation system that suggests songs based on cluster similarity and genre prediction.

## Installation and Setup
1. Install the required Python packages listed in `requirements.txt`.

## Usage
Run the Jupyter notebook provided in this repository to:
- Preprocess and explore the dataset.
- Cluster songs and visualize results.

---