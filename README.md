# YUGESWARI-0309

IMPLEMENTING K-MEANS CLUSTERING FROM SCRATCH AND EVOLUATING PERFOMANCE:
         
        This project focuses on implementing the K-Means clustering algorithm entirely from scratch using only NumPy, without relying on high-level libraries such as scikit-learn for the clustering logic. The goal is to help you understand the fundamental mechanics of how the K-Means algorithm works, including initialization, distance computation, cluster assignment, centroid updates, and convergence behavior.


METHODOLOGY:

        1. Dataset Generation

Use make_blobs from scikit-learn to generate:

500 samples

4 cluster centers

standard deviation = 1.5


Store the data (X) for clustering.



---

2. K-Means Implementation from Scratch

2.1 Initialization

Choose one:

Random Initialization
– Randomly pick K data points as initial centroids
OR

K-Means++ Initialization
– Choose the first centroid randomly
– For each subsequent centroid, choose points with probability proportional to their squared distance from nearest existing centroid.


2.2 Distance Calculation

Compute Euclidean distance between each data point and each centroid.

2.3 Cluster Assignment Step

Assign each data point to the nearest centroid.

2.4 Centroid Update Step

For each cluster, compute the mean of the assigned points.

2.5 Convergence Check

Repeat until:

centroids stop changing, or

max iterations reached (e.g., 100).


2.6 Compute Inertia

At every iteration:

calculate the sum of squared distances of each point to its assigned centroid.


Store all inertia values for visualization.


---

3. Visualization (Scratch Implementation)

Create:

Scatter plot of final clusters

Line plot of inertia vs iterations


Save images to Google Colab.


---

4. Scikit-learn KMeans Implementation

Run:

from sklearn.cluster import KMeans

Use:

KMeans(n_clusters=4, init='k-means++')

Fit on same dataset

Retrieve:

final inertia

final cluster labels

centroids



Visualize clusters for comparison.


---

5. Comparative Analysis

Write a detailed discussion comparing:

scratch inertia vs scikit-learn inertia,

convergence behavior,

impact of initialization strategy,

cluster interpretation based on centroid coordinates.



---

6. Final Report Structure

Write a text report with:

A. Introduction

What is K-Means?

Purpose of building from scratch.
