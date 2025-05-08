🔍 Overview
This assignment is divided into two major tasks:

Interactive Foreground Segmentation using K-Means Clustering

Face Recognition using K-Nearest Neighbors (K-NN)

Each task is designed to provide practical experience in applying core data mining techniques to image segmentation and recognition problems using both manual and library-based methods.

📌 Q1: Interactive Foreground Segmentation Using K-Means Clustering
Inspired by the Lazy Snapping technique, this task involves implementing a basic interactive image cut-out algorithm that segments an object from the background using human-provided seed pixels.

✅ Objectives
Implement K-Means Clustering from scratch

Extract and cluster foreground/background seed pixels

Compute class likelihoods using distance from cluster centroids

Generate segmentation masks by comparing class probabilities

🧠 Key Concepts
Clustering: RGB-based K-Means for seed pixel grouping

Probability Estimation: Negative exponential of Euclidean distance

Segmentation Rule: Assign pixel to class with higher likelihood (foreground or background)

🛠 Implementation Details
Seed Stroke Images: Red = foreground, Blue = background

Distance Metric: Euclidean

Experimentation: Try multiple N values (e.g., 16, 32, 64)

Likelihood Weighting: Fixed wk = 0.1

📊 Evaluation
Visual segmentation outputs for all test images

Result comparison for different N values

Report on effects of removing square operation in distance metric

📌 Q2: Face Recognition Using K-NN
Utilizing a simplified CMU PIE dataset, this task involves implementing a face recognition system from scratch using K-NN and comparing it with Scikit-learn classifiers.

✅ Objectives
Normalize and split the dataset into train/test sets

Implement K-NN from scratch with support for:

Euclidean distance

Cosine similarity

Evaluate performance for different k values: 2, 5, 7, 11

Compare with SVM and GaussianNB using Scikit-learn

Perform PCA and visualize faces in 3D

🧠 Key Concepts
Normalization: Each image vector scaled to unit norm

Distance Metrics: Both Euclidean and cosine implemented manually

Dimensionality Reduction: PCA for visualization

🛠 Implementation Details
Dataset Shape: 1700 samples × 1024 features

Split Strategy: 150 training and 20 testing images per subject (default)

Alternative Setup: 100 training and 70 testing per subject

Libraries Allowed: Only for PCA, SVM, and GaussianNB (Scikit-learn)

📊 Evaluation
Accuracy scores for K-NN with each k and distance metric

Performance drop/increase with smaller training size

Accuracy comparison with SVM and GaussianNB

3D plots of PCA-transformed data

