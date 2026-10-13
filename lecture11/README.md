# Lecture #11 (Dimensionality Reduction and Representation)

This folder contains the supporting material used during Lecture #11 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 12 November 2026**.

## Overview

This lecture covers essential dimensionality reduction techniques for high-dimensional data analysis and visualization. All examples are provided as interactive Jupyter Notebooks with detailed explanations, mathematical foundations, code implementations, and comprehensive visualizations.

## Content Structure

### Core Dimensionality Reduction Notebooks

#### 1. **Principal Component Analysis (PCA)** (`ex01_principal_component_analysis.ipynb`)

- **Learning Objectives**: Understanding PCA from mathematical foundations to practical implementation
- **Techniques Covered**:
  - Covariance matrix computation and visualization
  - Eigenvalue and eigenvector calculation
  - Principal component extraction
  - Variance explained analysis
  - Second-order equation visualization for reduced dimensions
- **Key Tools**: NumPy, pandas, seaborn, matplotlib, custom visualization functions
- **Dataset**: Blood pressure measurements (Systolic and Diastolic)
- **Practical Applications**: Medical data analysis, feature extraction, data compression

#### 2. **Linear Discriminant Analysis (LDA)** (`ex02_linear_discriminant_analysis.ipynb`)

- **Learning Objectives**: Supervised dimensionality reduction for classification tasks
- **Techniques Covered**:
  - Within-class scatter matrix computation
  - Between-class scatter matrix computation
  - Fisher's discriminant ratio maximization
  - LDA vs PCA comparison
  - Class separation visualization
- **Key Tools**: scikit-learn LDA, NumPy, matplotlib, custom scatter matrix functions
- **Dataset**: Breast Cancer Wisconsin dataset (30 features, binary classification)
- **Practical Applications**: Medical diagnosis, pattern recognition, supervised feature extraction

#### 3. **t-Distributed Stochastic Neighbor Embedding (t-SNE)** (`ex03_t_distributed_stochastic_neighbor_embedding.ipynb`)

- **Learning Objectives**: Non-linear dimensionality reduction for visualization
- **Techniques Covered**:
  - Pairwise distance matrix computation and visualization
  - t-SNE algorithm implementation
  - Perplexity parameter tuning
  - High-dimensional to 2D embedding
  - Initial random embedding visualization
- **Key Tools**: scikit-learn TSNE, NumPy, matplotlib, seaborn heatmaps
- **Dataset**: Breast Cancer Wisconsin dataset
- **Practical Applications**: High-dimensional data visualization, cluster discovery, exploratory data analysis

#### 4. **Dimensionality Reduction Comparison** (`ex04_dimensionality_reduction.ipynb`)

- **Learning Objectives**: Comparative analysis of PCA, LDA, and t-SNE techniques
- **Techniques Covered**:
  - Side-by-side visualization of three methods
  - Performance comparison on image features
  - Understanding strengths and limitations of each method
  - Feature extraction from deep learning models
- **Key Tools**: scikit-learn (PCA, LDA, TSNE), NumPy, matplotlib
- **Dataset**: ResNet50 features from cat and dog images (2048 dimensions → 2D)
- **Practical Applications**: Method selection, comparative analysis, visual exploration

#### 5. **Dynamic Interactive Visualization** (`ex05_dynamic_plot.ipynb`)

- **Learning Objectives**: Creating interactive dashboards for dimensionality reduction results
- **Techniques Covered**:
  - Dash web application development
  - Interactive scatter plots with tooltips
  - Real-time data visualization
  - Custom styling and layout design
- **Key Tools**: Dash, Plotly, pandas, custom callback functions
- **Dataset**: Cat and dog image features with metadata
- **Practical Applications**: Interactive data exploration, presentation dashboards, web-based analytics

#### 6. **Feature Extraction Pipeline** (`ex06_features_extractor.ipynb`)

- **Learning Objectives**: Extracting deep learning features for dimensionality reduction
- **Techniques Covered**:
  - Custom PyTorch Dataset implementation
  - Pretrained ResNet50 feature extraction
  - Image preprocessing and transformation
  - Batch processing with DataLoader
  - Feature and label persistence (.npy format)
- **Key Tools**: PyTorch, torchvision, PIL, NumPy, ResNet50 pretrained model
- **Dataset**: Cat and dog images (RGB, resized to 224×224)
- **Practical Applications**: Transfer learning, feature engineering, image analysis preprocessing

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each dimensionality reduction technique
- 🔍 **Mathematical Foundations** with covariance matrices, eigenvectors, and scatter matrices
- 💻 **Hands-on Code Examples** with detailed comments and explanations
- 📊 **Interactive Visualizations** using matplotlib, seaborn, and Plotly
- 📈 **Comparative Analysis** showing strengths and weaknesses of each method
- 🎯 **Real-world Applications** including medical diagnosis and image classification
- ✅ **Best Practices** for parameter selection and method choice
- ⚠️ **Common Pitfalls** and troubleshooting guidance
- 📝 **Comprehensive Summaries** with key takeaways and decision frameworks

## Technical Requirements

- **Python 3.x** with data science and deep learning libraries
- **Core Libraries**: NumPy, pandas, matplotlib, seaborn, scikit-learn
- **Deep Learning**: PyTorch, torchvision, PIL
- **Interactive Visualization**: Dash, Plotly
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Data Files**: Image datasets and extracted features in `data/` folder (managed with DVC)

## Additional Resources

### Folders

- **`data/`**: Image datasets (cats_set, dogs_set) and extracted features (features.npy, labels.npy) - DVC managed

### Files

- **`data.dvc`**: Data Version Control file for dataset management
- **`.gitignore`**: Git ignore patterns for the lecture folder

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Foundation** (Ex 1-3): Master core techniques

   - PCA fundamentals → LDA for supervised learning → t-SNE for visualization

2. **Comparison & Selection** (Ex 4): Understanding trade-offs

   - Comparative analysis of PCA, LDA, and t-SNE on real data

3. **Advanced Applications** (Ex 5-6): Practical implementation
   - Interactive dashboards → Feature extraction pipeline

Each notebook builds upon concepts from previous ones, progressing from mathematical foundations to practical applications, creating a comprehensive understanding of dimensionality reduction essential for high-dimensional data analysis and machine learning.

## Usage Instructions

1. **Setup Environment**: Ensure all required Python libraries are installed (including PyTorch for Ex 6)
2. **Extract Features**: Run Ex 6 first to generate features.npy and labels.npy files
3. **Launch Notebooks**: Open notebooks in Jupyter or VS Code
4. **Follow Sequence**: Work through notebooks in the recommended order
5. **Experiment**: Modify parameters (e.g., n_components, perplexity) with your own data
6. **Interactive Dashboard**: Run Ex 5 to launch the Dash application for interactive exploration

## Key Concepts Covered

- **Linear Methods**: PCA (unsupervised), LDA (supervised)
- **Non-linear Methods**: t-SNE for complex manifold visualization
- **Feature Extraction**: Deep learning features from pretrained CNNs
- **Visualization Techniques**: Heatmaps, scatter plots, interactive dashboards
- **Mathematical Foundations**: Covariance matrices, eigendecomposition, scatter matrices
- **Practical Considerations**: When to use each method, parameter tuning, computational efficiency

This comprehensive collection provides both theoretical understanding and practical skills for effective dimensionality reduction in real-world data mining and machine learning applications.
