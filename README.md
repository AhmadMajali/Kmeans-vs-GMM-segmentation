# Kmeans-vs-GMM-segmentation
Palmprint Image Segmentation

This project implements and compares two popular unsupervised machine learning techniques—K-Means Clustering and Gaussian Mixture Models (GMM)—to perform image segmentation on palmprint images.
** Overview**

Segmentation is the process of partitioning a digital image into multiple segments to simplify its representation. In the context of palmprint recognition, this is a crucial preprocessing step used to isolate the hand from the background.

    K-Means: An iterative algorithm that partitions data into K clusters where each pixel belongs to the cluster with the nearest mean (centroid).

    GMM: A probabilistic model that assumes all data points are generated from a mixture of a finite number of Gaussian distributions with unknown parameters.

 **Features**

    Color Space Conversion: Converts images from BGR (OpenCV default) to RGB for accurate visualization.

    Feature Vectorization: Reshapes 2D images into 1D pixel arrays for clustering.

    Dual-Model Comparison: Side-by-side visualization of K-Means vs. GMM results.

    Automated Mask Generation: Produces binary masks that can be used for further image processing.

**Requirements**

Ensure you have Python installed, then install the necessary dependencies:
Bash

pip install opencv-python matplotlib scikit-learn numpy
