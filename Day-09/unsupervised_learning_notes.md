# Unsupervised Learning - Day 09

## What is Unsupervised Learning?

Unsupervised Learning is a type of Machine Learning where the model works with unlabeled data and discovers hidden patterns, structures, or relationships without predefined outputs.

### Key Characteristics

* No target variable (label) is provided.
* Finds hidden patterns in data.
* Used for grouping and pattern discovery.
* Useful when labeled data is unavailable.

---

## Difference Between Supervised and Unsupervised Learning

| Feature          | Supervised Learning        | Unsupervised Learning                |
| ---------------- | -------------------------- | ------------------------------------ |
| Labels Available | Yes                        | No                                   |
| Goal             | Prediction                 | Pattern Discovery                    |
| Output           | Predicted Value/Class      | Clusters/Patterns                    |
| Training Data    | Labeled                    | Unlabeled                            |
| Examples         | Classification, Regression | Clustering, Dimensionality Reduction |

---

# Clustering

Clustering is the process of grouping similar data points together based on their characteristics.

### Purpose

* Identify hidden groups in data.
* Understand customer behavior.
* Discover patterns automatically.

### Examples

* Customer Segmentation
* Fraud Detection
* Social Network Analysis
* Market Research

---

# K-Means Clustering

K-Means is one of the most widely used clustering algorithms.

## How K-Means Works

### Step 1

Choose the number of clusters (K).

### Step 2

Randomly initialize K cluster centroids.

### Step 3

Assign each data point to the nearest centroid.

### Step 4

Recalculate centroids based on assigned points.

### Step 5

Repeat until cluster assignments stop changing.

---

## Choosing the Value of K

The Elbow Method is commonly used.

### Elbow Method

* Run K-Means for multiple values of K.
* Calculate clustering error for each K.
* Plot the error graph.
* Select the point where the decrease in error starts slowing significantly.

---

# Hierarchical Clustering

Hierarchical Clustering creates a hierarchy of clusters represented as a tree structure called a dendrogram.

## Types

### Agglomerative (Bottom-Up)

* Each data point starts as its own cluster.
* Closest clusters are merged repeatedly.

### Divisive (Top-Down)

* Start with one large cluster.
* Split clusters recursively.

## Advantages

* No need to specify K initially.
* Easy visualization through dendrograms.

## Limitations

* Computationally expensive for large datasets.

---

# Dimensionality Reduction

Dimensionality Reduction reduces the number of features while preserving important information.

## Benefits

* Faster training
* Reduced storage requirements
* Better visualization
* Less noise in data

---

# Principal Component Analysis (PCA)

PCA is a dimensionality reduction technique that transforms data into a smaller set of variables called Principal Components.

## Objectives

* Reduce dimensions
* Preserve maximum variance
* Improve computational efficiency

## Working Principle

1. Standardize data.
2. Compute covariance matrix.
3. Calculate eigenvectors and eigenvalues.
4. Select principal components.
5. Transform original data.

## Advantages

* Faster computation
* Reduced complexity
* Better visualization
* Noise reduction

---

# Applications of Unsupervised Learning

* Customer Segmentation
* Recommendation Systems
* Fraud Detection
* Medical Diagnosis Research
* Market Basket Analysis
* Image Compression
* Social Network Analysis
* Document Categorization

---

# Conclusion

Unsupervised Learning helps discover hidden structures and relationships within unlabeled data. Techniques such as Clustering and PCA enable organizations to generate valuable insights and make data-driven decisions.
