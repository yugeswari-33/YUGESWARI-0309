# YUGESWARI-0309

IMPLEMENTING K-MEANS CLUSTERING FROM SCRATCH AND EVOLUATING PERFOMANCE:
         
        The code implements K-Means clustering from scratch using NumPy and compares it with Scikit-learn’s implementation. It generates synthetic datasets, runs K-Means with different centroid initializations, tracks inertia evolution, saves outputs, and plots results.

METHODOLOGY:

        1. Data Generation:
    - Uses make_blobs to create synthetic datasets with specified samples, centers, and standard deviation for testing K-Means.

2. K-Means Scratch Implementation:
    - Includes functions for centroid initialization (random_init, kmeans_pp_init), cluster assignment, centroid updates, and inertia computation.
    - Runs K-Means with both random and kmeans++ initializations for comparison.

3. Output and Evaluation:
    - Saves cluster labels, centroids, inertia histories, and plots cluster distributions and inertia evolution.
    - Compares scratch implementation results with Scikit-learn KMeans to validate correctness.

4. Reporting:
    - Generates a report summarizing dataset details, convergence status, final inertia values, and centroid coordinates for analysis.
