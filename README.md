# IPL Batsmen Clustering Project
## Overview
This project aims to analyze and cluster IPL batsmen based on their performance metrics using various clustering algorithms. The goal is to identify and categorize some of the best IPL batsmen of all time based on their strengths.

## Dataset
The dataset contains detailed ball-by-ball information from IPL matches, including the following columns:

id: Unique Match ID as per ESPNCricinfo
inning: Inning Number
over: Over Number
ball: Ball Number
batsman: Batsman on strike
non_striker: Batsman at non-striker
bowler: Bowler
batsman_runs: Runs off bat
extra_runs: Extra runs
total_runs: Total Runs
non_boundary: If there are overthrows
is_wicket: Is the delivery a wicket?
dismissal_kind: Type of dismissal
player_dismissed: Player who got dismissed
fielder: Fielder involved in the dismissal
extras_type: Type of extras
batting_team: Batting team
bowling_team: Bowling team
Project Structure
data/: Contains the dataset used for the analysis.
notebooks/: Jupyter notebooks used for data analysis, feature engineering, and clustering.
src/: Source code for data processing, feature extraction, and clustering algorithms.
results/: Contains the results of the clustering analysis.
README.md: Project documentation.

## Analysis and Results
Exploratory Data Analysis (EDA)
The EDA notebook (notebooks/eda.ipynb) provides insights into the data quality and distributions. Missing values were treated and relevant features were generated, including total runs scored, strike rate, etc.

Clustering Algorithms
The following clustering algorithms were applied to the dataset:

KMeans
DBSCAN
Hierarchical Clustering
The clustering results were evaluated using the silhouette score:

KMeans: 0.587181207076276
DBSCAN: -0.33097189234438534
Agglomerative Clustering: 0.5280415407860092
Visualizations
Visualizations of the clustered data are provided in the clustering notebook (notebooks/clustering.ipynb). These visualizations help in understanding the grouping of batsmen based on their performance metrics.

## Conclusion
The KMeans algorithm provided the best clustering performance with a silhouette score of 0.587. This project demonstrates the process of clustering IPL batsmen using various algorithms and highlights the importance of parameter tuning and data preprocessing.

## Future Work
Experiment with other clustering algorithms such as Gaussian Mixture Models and Spectral Clustering.
Improve the feature set by including additional performance metrics.
Perform parameter tuning for DBSCAN to achieve better results.
## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any changes.
