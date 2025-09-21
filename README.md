<p align="center"><img width="100%" src="ML/others/logo/torch_and_tf.svg" /></p>

--------------------------------------------------------------------------------


[![Build Status](https://travis-ci.com/aladdinpersson/Machine-Learning-Collection.svg?branch=master)](https://travis-ci.com/aladdinpersson/Machine-Learning-Collection) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[logo]: https://github.com/AladdinPerzon/Machine-Learning-Collection/blob/master/ML/others/logo/youtube_logo.png

# Machine Learning Collection
In this repository you will find tutorials and projects related to Machine Learning. I try to make the code as clear as possible, and the goal is be to used as a learning resource and a way to lookup problems to solve specific problems. For most I have also done video explanations on YouTube if you want a walkthrough for the code. If you got any questions or suggestions for future videos I prefer if you ask it on. This repository is contribution friendly, so if you feel you want to add something then I'd happily merge a PR :smiley:

This script performs a customer segmentation analysis on mall customer data.

Here's a breakdown of the steps:

Data Generation and Loading: Synthetic mall customer data is generated and saved to a CSV file, then loaded into a pandas DataFrame.
Exploratory Data Analysis (EDA): The script explores the data by:
Displaying the number of rows and columns.
Showing a sample of the data.
Generating descriptive statistics.
Checking for missing values.
Analyzing the distribution of age, annual income, and spending score, including separate analyses for male and female customers using histograms and boxplots.
Performing Kolmogorov-Smirnov tests to compare the distributions of age, income, and spending scores between genders.
Visualizing the median annual income by age group for both genders.
Examining the correlation between age and spending score using a joint plot and Pearson correlation.
Analyzing the correlation between age and annual income and age and spending score for both genders using scatter plots with linear regression lines.
Analyzing the correlation between annual income and spending score for both genders using scatter plots with linear regression lines.
Clustering Analysis: The script applies three different clustering algorithms to the numeric features (Age, Annual Income (k$), and Spending Score (1-100)):
K-Means: The optimal number of clusters is determined using the Elbow method and Silhouette analysis. Clustering is performed with 5 and 6 clusters, and the results are visualized and cluster sizes are shown.
DBSCAN: A grid search is performed to find the best eps and min_samples parameters based on the number of clusters and silhouette score. The results are visualized using heatmaps. Clustering is performed with the chosen parameters, and the resulting clusters and outliers are visualized.
Affinity Propagation: The optimal preference parameter is explored based on the silhouette score. Clustering is performed with the chosen preference, and the results are visualized and cluster sizes are shown.
Comparison of Clustering Results: The sizes of the clusters found by K-Means (with 6 clusters), DBSCAN, and Affinity Propagation are displayed side-by-side for comparison.
