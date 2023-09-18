# Ev-Driver-Clustering
This project aims to cluster electric vehicle drivers based on their driving behavior data provided by Lithion Power, a company that rents out batteries to e-vehicle drivers. The goal is to group drivers together based on their driving history and use these clusters to incentivize drivers. 

The dataset used in this project contains information on drivers, including their mean daily distance driven (mean_dist_day) and the percentage of time they exceeded the speed limit (mean_over_speed_perc). The clustering process is performed using the K-Means algorithm, which groups similar drivers together based on these two features.

Here is a brief overview of the steps taken in the project:

Data Preparation: The dataset is loaded and examined for any missing values or anomalies. Fortunately, there are no missing values in the dataset.

Feature Selection: The 'id' column is dropped from the dataset as it is not relevant for clustering.

Clustering: K-Means clustering is applied to the dataset. Initially, two clusters are created, and the center vectors for these clusters are obtained. Later, the number of clusters is increased to four, and the center vectors for these clusters are also obtained.

Visualization: The clusters are visualized on a scatter plot using the seaborn library. Each point on the plot represents a driver, with different colors indicating different clusters.

Evaluation: The silhouette score is calculated to measure the quality of the clusters. A higher silhouette score indicates that the data points within the clusters are well-separated and distinct.

Incentivization: The clusters can be used to group drivers with similar driving behavior. Lithion Power can then offer incentives or pricing models tailored to each cluster, encouraging drivers to adopt safer and more efficient driving habits.

In summary, this project demonstrates how clustering can be used to segment electric vehicle drivers based on their driving behavior, allowing Lithion Power to offer personalized incentives and pricing models to encourage safe and efficient driving practices among their customers.


