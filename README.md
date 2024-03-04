# Song clustering with unsupervised ML WBS, creating playlists from 5000 spotify songs
 A project within the Data Science Bootcamp at WBS Coding School

## The Task and Overview

Moosic is a little start-up that creates playlists curated by music experts and specialists in old and new trends. Users can subscribe to their website and listen to these playlists through their preferred Music App.
Use Data Science to add a degree of automatisation to the creation of playlists. Build a first prototype model how to cluster songs for playlists.
Use KMeans to build the model.

### Steps:
- Cleaning the data, use of numeric values only
- Scaling the features. After tests with MinMax and Standard Scaler, the robust scaler with a quantile range 10,90 delivered the best peformance.
- PCA to determine combination of most relevant features with a cumulated variance of 0.95.
- Determination of k with inertia and Silhouette Scores. To create more distinct playlist cluster, we set k to a small number of 6. This created large clusters with several hundert songs.
- Filter the playlits and keep the only top 50 songs with smallest distance to the core of each cluster


## Data Source
A [dataset](https://github.com/HannePruefer/Unsupervised_ML_clustering-Data/blob/main/6.3.3_spotify_5000_songs.csv) with 5000 song titles with Spotify Audio Features to describe them

## Tools used
- Python pandas
- Pyhton SciKit Learn 
- Plotly for visualization 

This is the [notebook](https://github.com/HannePruefer/Unsupervised_ML_clustering-Data/blob/main/Spotify_Playlists.ipynb) containing the clustering

[Here](https://github.com/HannePruefer/Unsupervised_ML_clustering-Data/blob/main/Moosic%20Playlists.pdf) is also a presentation on the project



## Co-Authors
- [Tilman Vogel](https://github.com/tvogel)
- Sebastian Foth 
