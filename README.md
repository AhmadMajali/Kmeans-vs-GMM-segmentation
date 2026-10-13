# K-Means vs. GMM: Palmprint Image Segmentation

This project implements and compares two unsupervised machine learning methods, K-Means clustering and Gaussian Mixture Models (GMM), for segmenting palmprint images.

## Result

![Original image, K-Means segmentation and GMM segmentation](images/segmentation_results.png)

Left to right: the original image, the K-Means mask and the GMM mask. On this example, GMM gives a cleaner hand outline, while K-Means leaves stray specks along the bottom edge. The two masks have opposite colours because cluster labels are arbitrary. This is one example image, not a benchmark.

## Overview

Segmentation partitions an image into regions to simplify its representation. In palmprint recognition it is a key preprocessing step, used to isolate the hand from the background.

- **K-Means:** an iterative algorithm that splits the data into K clusters, assigning each pixel to the cluster with the nearest mean (centroid).
- **GMM:** a probabilistic model that assumes the data comes from a mixture of a finite number of Gaussian distributions with unknown parameters.

## Features

- **Colour space conversion:** converts images from BGR (OpenCV's default) to RGB for correct display.
- **Feature vectorisation:** reshapes the 2D image into a list of pixels for clustering.
- **Side-by-side comparison:** shows the K-Means and GMM results next to the original.
- **Mask generation:** produces binary masks that can be used in further image processing.

## Requirements

Install the dependencies:

```bash
pip install opencv-python matplotlib scikit-learn numpy
```

**Important:** update the image path in the code to point to an image on your machine.
