🎵 Spotify Music Recommendation System

This project is a data-driven Spotify Music Recommendation System built using Python, Pandas, Scikit-learn, and Matplotlib.
It analyzes and clusters songs based on their audio features and provides song recommendations using K-Means Clustering.

🚀 Project Overview

This system uses Spotify’s music dataset to:

Preprocess and clean the data

Analyze relationships between audio features

Identify song patterns and similarities using K-Means Clustering

Visualize clusters using PCA (Principal Component Analysis)

Recommend similar songs based on cluster similarity

🧠 Key Features

📊 Data Preprocessing: Handles missing values, duplicates, and date formatting

🔍 Feature Analysis: Visualizes feature distributions and correlations

🤖 K-Means Clustering: Groups songs based on their musical characteristics

🎨 Visualizations: Generates histograms, heatmaps, and PCA-based scatter plots

💡 Recommendation Engine: Suggests similar songs within the same cluster

💾 Output File: Saves the final dataset with cluster labels

🧰 Technologies Used
Category	Libraries/Tools
Data Handling	pandas, numpy
Visualization	matplotlib, seaborn
Machine Learning	scikit-learn (StandardScaler, KMeans, PCA)
Environment	Python 3.x, Jupyter/Colab/VS Code
📂 Dataset

Make sure to have the Spotify Dataset CSV file in your working directory.

📁 File Name: spotify dataset.csv
🗂️ Example Path: /content/drive/MyDrive/spotify dataset.csv

Dataset Columns (example):

track_id, track_name, track_artist, track_popularity, playlist_genre,
danceability, energy, speechiness, acousticness, instrumentalness,
liveness, valence, tempo, duration_ms, track_album_release_date

⚙️ How to Run

Clone the Repository

git clone https://github.com/<your-username>/spotify-recommendation-system.git
cd spotify-recommendation-system


Install Dependencies

pip install -r requirements.txt


(You can generate requirements.txt using pip freeze > requirements.txt)

Place the Dataset

Copy spotify dataset.csv into the same directory as the script.

Run the Script

python spotify_recommendation_system.py

📈 Workflow Summary

Data Preprocessing

Handles missing values & duplicates

Extracts release year from the release date

Exploratory Data Analysis

Plots distributions of audio features

Visualizes correlations between features

Clustering

Standardizes data using StandardScaler

Finds the optimal cluster number using the Elbow Method

Applies K-Means to group similar songs

Visualization

Uses PCA to project clusters into 2D for visualization

Recommendation System

Finds songs in the same cluster as a given track (e.g., “Blinding Lights”)

Returns the top 10 similar songs based on cluster and popularity

Save Results

Exports clustered dataset to spotify_with_clusters.csv

🧩 Example Output

Recommendation Example:

Recommendation for 'Blinding Lights' (Cluster 2):
          track_name          track_artist     playlist_genre  track_popularity
32     Levitating           Dua Lipa               pop                  89
56     Save Your Tears      The Weeknd             pop                  88
91     Don’t Start Now      Dua Lipa               pop                  85
...

🖼️ Visual Outputs

Feature Distributions: Understands range and skewness of features

Correlation Heatmap: Shows relationships between numerical attributes

Elbow Plot: Helps choose the optimal number of clusters

PCA Scatter Plot: Displays clusters in 2D space

Cluster-Genre Bar Chart: Explores genre distribution per cluster

📊 Output Files
File Name	Description
spotify_with_clusters.csv	Final dataset with assigned cluster labels
spotify dataset.csv	Input dataset (you must provide this)
🧠 Future Improvements

Implement a content-based filtering approach using cosine similarity

Integrate Spotify Web API for real-time recommendations

Deploy as a web app using Streamlit or Flask

Include user feedback-based tuning of cluster recommendations
