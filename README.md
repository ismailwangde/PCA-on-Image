# PCA on Face Images

## Overview
This project demonstrates the application of **Principal Component Analysis (PCA)** for:
- Dimensionality reduction of face images.
- Visualization of important features in the dataset.
- Reconstruction of images using reduced dimensions.
- Real-time image capture and processing with OpenCV.

---

## Steps in the Project

### 1. Loading and Analyzing Face Data
- **Dataset**: Uses the Olivetti Faces dataset from `sklearn.datasets`.
- **Objective**: Apply PCA to reduce dimensions while preserving maximum variance.
- **Key Visualizations**:
  - Mean face to analyze average features.
  - Principal components to highlight key features of the data.
  - Explained variance ratio to determine the contribution of each component.

### 2. Capturing Images Using OpenCV
- The script captures images in real-time using a webcam.
- Images are resized to a fixed dimension and stored in a specified directory.
- Each captured image is labeled and displayed during the process.
- Collects **50 samples** for analysis.

### 3. Preprocessing Captured Images
- Converts captured images into numerical arrays.
- Normalizes the data for consistent analysis.
- Reduces dimensions using PCA, retaining only the top **20 components**.

### 4. Image Reconstruction
- Reconstructs images from the reduced-dimensional data using PCA inverse transformation.
- Visualizes the difference between original and reconstructed images.

### 5. Visualization
- Plots **cumulative explained variance ratio** to analyze the variance captured.
- Displays **principal components** of both the Olivetti dataset and the captured images.

---

## Results
- **Dimensionality Reduction**: PCA effectively reduces dimensions while preserving key information.
- **Principal Components**: Highlights significant features of the dataset.
- **Reconstructed Images**: Demonstrates the impact of PCA on image quality and compression.
