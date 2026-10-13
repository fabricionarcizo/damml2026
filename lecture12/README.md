# Lecture #12 (Anomaly and Outlier Detection)

This folder contains the supporting material used during Lecture #12 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 19 November 2026**.

## Overview

This lecture covers comprehensive anomaly detection techniques essential for identifying unusual patterns, outliers, and anomalies in datasets. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and visualizations.

## Content Structure

### Core Anomaly Detection Notebooks

#### 1. **Univariate Parametric Methods** (`ex01_univariate_parametric.ipynb`)

- **Learning Objectives**: Understanding parametric approaches for detecting anomalies in single-variable datasets
- **Techniques Covered**:
  - Normal Distribution Method (3σ rule)
  - Interquartile Range (IQR) Method
  - Grubb's Test for outlier detection
  - Statistical threshold determination
- **Key Tools**: SciPy statistics, NumPy, pandas, matplotlib, seaborn
- **Practical Applications**: Quality control, sensor data validation, financial fraud detection

#### 2. **Multivariate Parametric Methods** (`ex02_multivariate_parametric.ipynb`)

- **Learning Objectives**: Detecting anomalies in multi-dimensional datasets using parametric approaches
- **Techniques Covered**:
  - Mahalanobis Distance calculation
  - Chi-squared threshold determination
  - Gaussian Mixture Models (GMM)
  - Covariance-based anomaly detection
- **Key Tools**: scikit-learn GaussianMixture, SciPy spatial distance functions
- **Practical Applications**: Multivariate quality control, customer behavior analysis, system health monitoring

#### 3. **Non-Parametric Methods** (`ex03_non_parametric.ipynb`)

- **Learning Objectives**: Distribution-free approaches for anomaly detection
- **Techniques Covered**:
  - Histogram-based anomaly detection
  - Kernel Density Estimation (KDE)
  - Percentile-based thresholding
  - Density-based outlier scoring
- **Key Tools**: scikit-learn KernelDensity, NumPy histogram functions
- **Practical Applications**: Non-normal distributions, unknown data distributions, robust detection

#### 4. **Proximity-Based Methods** (`ex04_proximity_based_methods.ipynb`)

- **Learning Objectives**: Distance and density-based anomaly identification
- **Techniques Covered**:
  - DB(r, π)-outlier detection method
  - Local Outlier Factor (LOF)
  - Nearest neighbor approaches
  - Density-based outlier scoring
- **Key Tools**: scikit-learn LocalOutlierFactor, NearestNeighbors
- **Practical Applications**: Spatial anomaly detection, network intrusion detection, point cloud analysis

#### 5. **Clustering-Based Methods** (`ex05_clustering_based_methods.ipynb`)

- **Learning Objectives**: Leveraging clustering algorithms for anomaly detection
- **Techniques Covered**:
  - Distance to Cluster Centroid (KMeans-based)
  - Density-Based Spatial Clustering (DBSCAN)
  - Cluster-Based Local Outliers (LOF)
  - Multiple clustering approaches comparison
- **Key Tools**: scikit-learn KMeans, DBSCAN, LocalOutlierFactor
- **Practical Applications**: Customer segmentation outliers, manufacturing defects, network security

#### 6. **One-Class SVM** (`ex06_one_class_svm.ipynb`)

- **Learning Objectives**: Machine learning approach for novelty and anomaly detection
- **Techniques Covered**:
  - One-Class Support Vector Machine (SVM)
  - RBF kernel for non-linear decision boundaries
  - Hyperparameter tuning (nu, gamma)
  - Decision boundary visualization
- **Key Tools**: scikit-learn OneClassSVM
- **Practical Applications**: Novelty detection, one-class classification, rare event detection

#### 7. **Autoencoders for Anomaly Detection** (`ex07_autoencoders_anomaly_detector.ipynb`)

- **Learning Objectives**: Deep learning approach using neural network reconstruction error
- **Techniques Covered**:
  - Autoencoder architecture design
  - Reconstruction error calculation
  - Threshold-based anomaly identification
  - Neural network training for anomaly detection
- **Key Tools**: TensorFlow/Keras, neural network layers, Adam optimizer
- **Practical Applications**: Complex pattern anomalies, high-dimensional data, image/signal anomaly detection

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each topic
- 🔍 **Step-by-step Explanations** with theoretical background
- 💻 **Hands-on Code Examples** with detailed comments
- 📊 **Interactive Visualizations** using matplotlib with custom color schemes
- 📈 **Statistical Analysis** and validation methods
- 🎯 **Real-world Applications** and use case scenarios
- ✅ **Best Practices** and implementation guidelines
- ⚠️ **Common Pitfalls** and how to avoid them
- 🎨 **Consistent Plot Design** with professional color palette
- 📝 **Comprehensive Summaries** with key takeaways

## Technical Requirements

- **Python 3.x** with data science libraries
- **Core Libraries**: pandas, NumPy, matplotlib, seaborn, scikit-learn, SciPy
- **Deep Learning**: TensorFlow/Keras (for autoencoder notebook)
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Datasets**: Built-in datasets (seaborn tips, scikit-learn make_blobs)

## Additional Resources

### Python Scripts

Original Python scripts are also available for command-line execution:

- `ex01_univariate_parametric.py`
- `ex02_multivariate_parametric.py`
- `ex03_non_parametric.py`
- `ex04_proximity_based_methods.py`
- `ex05_clustering_based_methods.py`
- `ex06_one_class_svm.py`
- `ex07_autoencoders_anomaly_detector.py`

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Parametric Foundation** (Ex 1-2): Start with statistical approaches

   - Univariate methods → Multivariate methods

2. **Non-Parametric & Distance-Based** (Ex 3-4): Distribution-free approaches

   - Histogram/KDE methods → Proximity-based detection

3. **Advanced Clustering & ML** (Ex 5-7): Machine learning approaches
   - Clustering methods → One-Class SVM → Deep learning autoencoders

Each notebook builds upon concepts from previous ones, creating a comprehensive understanding of anomaly detection techniques ranging from classical statistical methods to modern deep learning approaches.

## Usage Instructions

1. **Setup Environment**: Ensure all required Python libraries are installed
2. **Launch Notebooks**: Open notebooks in Jupyter or VS Code
3. **Follow Sequence**: Work through notebooks in the recommended order
4. **Run Python Scripts**: Alternatively, execute `.py` files directly from terminal
5. **Experiment**: Modify parameters and test with your own data

## Key Concepts Covered

- **Parametric vs. Non-Parametric**: Understanding when to use assumption-based vs. distribution-free methods
- **Distance-Based Detection**: Leveraging spatial relationships for anomaly identification
- **Density-Based Approaches**: Identifying anomalies in low-density regions
- **Machine Learning Methods**: Using supervised and unsupervised learning for anomaly detection
- **Deep Learning**: Neural network reconstruction for complex pattern anomalies
- **Threshold Selection**: Statistical and percentile-based threshold determination
- **Evaluation Metrics**: Assessing anomaly detection performance

This comprehensive collection provides both theoretical understanding and practical skills for effective anomaly detection in real-world data mining and machine learning applications, from simple univariate cases to complex high-dimensional scenarios.
