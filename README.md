Amazon Music Unsupervised Learning – Cluster Analysis
📌 Project Overview

This project explores music track data from Amazon Music using unsupervised learning techniques to uncover patterns and group similar tracks. The goal is to identify clusters of songs based on their audio features, which can help in playlist creation, recommendation systems, or music analysis.

🗂 Dataset
Contains various audio features per track, including:
duration_ms, danceability, energy, loudness, speechiness, acousticness, instrumentalness, liveness, valence, tempo
Some features may contain outliers and require scaling for model-based clustering.
🛠 Tools & Libraries
Python (primary programming language)
Pandas, NumPy – data manipulation
Scikit-learn – preprocessing, PCA, KMeans clustering
Seaborn & Matplotlib – visualization
Optional: Power BI for dashboarding
⚙️ Methodology
Data Cleaning & Preprocessing
Checked for missing values and handled them using cluster-wise mean imputation.
Outliers were analyzed using boxplots per cluster.
Feature scaling applied for clustering (StandardScaler).
Dimensionality Reduction
Applied PCA to reduce high-dimensional data to 2 components for visualization and improved clustering.
Clustering
Used KMeans clustering to group songs into distinct clusters.
Determined optimal number of clusters using the Elbow Method and Silhouette Score.
Assigned each track a Cluster_Label for analysis.
Cluster Profiling
Calculated cluster-wise mean/median for all features to understand characteristic differences between clusters.
Visualized distributions with boxplots.
Exporting Results
Final clustered dataframe saved as music_clustered_final.csv.
Cluster profiles can be exported separately for reporting.
📊 Insights
Each cluster groups tracks with similar audio characteristics, such as high energy, tempo, or acousticness.
Boxplots reveal feature distributions and outliers across clusters.
Cluster profiles help in interpreting each group and can guide playlist recommendations or marketing strategies.
⚡ Usage
Load the music_clustered_final.csv file in Python or Power BI.
Explore clusters, analyze feature distributions, or use for recommendation systems.
Adjust preprocessing, scaling, or clustering parameters as needed for new datasets.
