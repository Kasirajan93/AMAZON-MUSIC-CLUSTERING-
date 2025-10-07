# AMAZON-MUSIC-CLUSTERING-

🎵 Amazon Music Clustering
-
🧠 Overview
-
With millions of songs on streaming platforms like Amazon Music, manually categorizing each track by genre or mood is nearly impossible.

This project applies unsupervised machine learning to automatically group songs based on audio features such as tempo, energy, danceability, loudness, and more — uncovering hidden patterns that represent genres, moods, or sound styles.

Through clustering, we enable data-driven insights into music preferences, playlist curation, and trend discovery — all without human labels.

🚀 Key Features
-
✅ Automatic Song Grouping using K-Means Clustering
✅ Interactive Dashboard built with Streamlit
✅ Dimensionality Reduction (PCA / t-SNE) for visualization
✅ Cluster Evaluation with Silhouette & Davies-Bouldin Scores
✅ Dynamic Feature Scaling (Standard / MinMax)
✅ Downloadable Clustered Dataset (CSV)
✅ Visual Analytics: Elbow Curves, Heatmaps, Boxplots

🧩 Project Pipeline
-
1️⃣ Data Exploration & Cleaning
-
Load and inspect dataset: amazon_music_clusters_all_methods.csv

Handle missing values, remove duplicates, and drop irrelevant columns

Identify numeric features for clustering

Apply scaling using StandardScaler or MinMaxScaler

2️⃣ Feature Selection
-
Selected features include:

danceability, energy, loudness, speechiness,
acousticness, instrumentalness, liveness, valence,
tempo, duration_ms

3️⃣ Dimensionality Reduction
-
PCA (Principal Component Analysis) for linear structure

t-SNE (optional) for nonlinear relationships

Used for 2D and 3D cluster visualization

4️⃣ Clustering Techniques
-
K-Means (primary algorithm)

Determine optimal k using Elbow & Silhouette methods

(Optional extensions)

DBSCAN for density-based clustering

Hierarchical Clustering for dendrogram visualization

5️⃣ Cluster Evaluation Metrics
-
Metric	Meaning	Goal
Silhouette Score	Cluster separation quality	Higher = Better
Davies-Bouldin Index	Intra-cluster similarity	Lower = Better
Inertia	Cluster compactness	Lower = Better

6️⃣ Visualization
-
📉 Elbow Curve – Find best number of clusters

🎨 PCA Scatter Plot (2D/3D) – View cluster separations

🔥 Heatmap – Compare average feature values by cluster

📊 Boxplots – Analyze feature distributions per cluster

7️⃣ Final Analysis
-
Assign cluster labels to the dataset

Profile clusters, e.g.:

Cluster 0 → High energy + loudness → Party Tracks

Cluster 1 → High acousticness + valence → Chill Vibes

Export final clustered data as amazon_music_clustered_data.csv


📈 Example Dashboard Preview
-
The Streamlit app provides an interactive interface for exploring song clusters.

Main Features:

Sidebar with scaling, cluster count, and visualization options

Real-time cluster evaluation metrics

PCA visualizations (2D & 3D using Plotly)

Feature-level comparison by cluster

Data download functionality

🧮 Tech Stack
-
Category	Tools / Libraries
Language	Python 3.x
Data Handling	pandas, NumPy
Machine Learning	scikit-learn
Visualization	matplotlib, seaborn, plotly
App Framework	Streamlit
Other	PCA, KMeans, Silhouette & DB Index

💡 Business Use Cases
-
🎧 Personalized Playlist Generation
-
Automatically create playlists of songs with similar sound profiles.

🔍 Music Recommendation Systems
-
Suggest new tracks to users based on their favorite clusters.

🎤 Artist Analysis
-
Help artists identify similar-sounding competitors or collaborators.

📈 Market & Trend Insights
-
Cluster listening patterns to understand audience behavior or regional trends.


🧠 Insights & Results
-
✅ Discovered distinct musical clusters such as:

Cluster 0: High energy, loudness → Workout / Party Tracks

Cluster 1: Acoustic, low energy → Chill / Relaxing Music

Cluster 2: Speech-heavy → Podcasts / Rap / Talk

✅ Improved interpretability using PCA visualizations.
✅ Achieved strong separation with high Silhouette scores.
✅ Delivered an interactive Streamlit interface for exploration
