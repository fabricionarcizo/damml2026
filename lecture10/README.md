# Lecture #10 (Clustering)

This folder contains the supporting material used during Lecture #10 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 05 November 2026**.

## Overview

This lecture covers fundamental clustering techniques and evaluation methods essential for unsupervised learning in data mining and machine learning. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and visualizations.

## Content Structure

### Core Clustering Algorithms

#### 1. **K-Means Clustering** (`ex01_k_means_clustering.ipynb`)

- **Learning Objectives**: Understanding the K-Means algorithm from scratch
- **Techniques Covered**:
  - K-Means algorithm implementation from first principles
  - Centroid initialization strategies
  - Cluster assignment and centroid update steps
  - Iterative convergence process
  - Distance-based clustering visualization
- **Key Tools**: NumPy for computational operations, matplotlib for visualizations, scikit-learn for data generation
- **Practical Applications**: Customer segmentation, image compression, pattern recognition

#### 2. **Elbow Method** (`ex02_elbow_method.ipynb`)

- **Learning Objectives**: Determining the optimal number of clusters using the elbow method
- **Techniques Covered**:
  - Within-Cluster Sum of Squares (WCSS) calculation
  - Inertia analysis across different k values
  - Elbow point detection using KneeLocator
  - Automated optimal k selection
  - Visual interpretation of elbow plots
- **Key Tools**: scikit-learn KMeans, kneed library for knee detection, matplotlib
- **Practical Applications**: Model selection, hyperparameter tuning, cluster validation

#### 3. **T-Shirt Clustering** (`ex03_tshirt_clustering.ipynb`)

- **Learning Objectives**: Applying K-Means to real-world sizing problems with outlier handling
- **Techniques Covered**:
  - K-Means clustering on Star Wars character data
  - Statistical outlier detection and removal
  - Standard deviation-based filtering
  - Before/after comparison of clustering results
  - Data cleaning impact on cluster quality
- **Key Tools**: pandas for data manipulation, scikit-learn KMeans, matplotlib
- **Practical Applications**: Product sizing, customer categorization, inventory management

#### 4. **Hierarchical Clustering** (`ex04_hierarchical_clustering.ipynb`)

- **Learning Objectives**: Understanding hierarchical/agglomerative clustering approaches
- **Techniques Covered**:
  - Agglomerative clustering implementation
  - Dendrogram generation and interpretation
  - Linkage methods (ward, complete, average)
  - Cluster hierarchy visualization
  - Distance-based cluster formation
- **Key Tools**: scikit-learn AgglomerativeClustering, scipy hierarchy functions, matplotlib
- **Practical Applications**: Taxonomy creation, document clustering, social network analysis

### Advanced Clustering Techniques

#### 5. **Dendrograms Comparison** (`ex05_dendrograms.ipynb`)

- **Learning Objectives**: Comparing different linkage methods in hierarchical clustering
- **Techniques Covered**:
  - Six linkage methods: single, complete, average, weighted, centroid, ward
  - Dendrogram visualization for each method
  - Cluster assignment based on distance thresholds
  - Comparative analysis of linkage strategies
  - Method selection guidelines
- **Key Tools**: scipy hierarchy functions, matplotlib subplots, rose-pine theme styling
- **Practical Applications**: Method selection, cluster structure analysis, hierarchical relationship discovery

#### 6. **Silhouette Score Evaluation** (`ex06_silhouette_score.ipynb`)

- **Learning Objectives**: Evaluating clustering quality using silhouette metrics
- **Techniques Covered**:
  - Silhouette score calculation for clustering quality
  - K-Means vs Agglomerative Clustering comparison
  - Within-cluster cohesion measurement
  - Between-cluster separation analysis
  - Quality metric interpretation
- **Key Tools**: scikit-learn silhouette_score and silhouette_samples, matplotlib
- **Practical Applications**: Cluster validation, algorithm comparison, quality assurance

#### 7. **K-Means Evaluation** (`ex07_k_means_evaluation.ipynb`)

- **Learning Objectives**: Systematic evaluation of K-Means with different k values
- **Techniques Covered**:
  - Within-Cluster Sum of Squares (WCSS) evaluation
  - Multiple k-value comparison (k=2, 3, 4)
  - Visual assessment of cluster quality
  - Trade-off analysis between k and WCSS
  - Cluster compactness measurement
- **Key Tools**: scikit-learn KMeans, matplotlib subplots for comparison
- **Practical Applications**: Model optimization, hyperparameter selection, clustering performance analysis

#### 8. **Feature Analysis** (`ex08_feature_analysis.ipynb`)

- **Learning Objectives**: Analyzing feature importance and cluster characteristics
- **Techniques Covered**:
  - Heatmap visualization of cluster features
  - Average feature value calculation per cluster
  - Cluster characterization and interpretation
  - Feature-based cluster differentiation
  - Multi-dimensional cluster analysis
- **Key Tools**: seaborn heatmaps, pandas groupby operations, scikit-learn on Iris dataset
- **Practical Applications**: Cluster interpretation, feature importance analysis, segmentation insights

#### 9. **DBSCAN Clustering** (`ex09_dbscan_clustering.ipynb`)

- **Learning Objectives**: Understanding density-based spatial clustering and comparing it with K-Means
- **Techniques Covered**:
  - K-Means clustering on anisotropic data
  - DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
  - Feature standardization for density-based methods
  - Handling arbitrary-shaped clusters
  - Noise point detection and outlier identification
  - Comparison of centroid-based vs. density-based clustering
- **Key Tools**: scikit-learn DBSCAN and KMeans, StandardScaler, pandas, matplotlib
- **Practical Applications**: Spatial data analysis, anomaly detection, cluster discovery without predefined k

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each clustering technique
- 🔍 **Step-by-step Explanations** with algorithmic details
- 💻 **Hands-on Code Examples** with comprehensive comments
- 📊 **Interactive Visualizations** using matplotlib and seaborn
- 📈 **Evaluation Metrics** for cluster quality assessment
- 🎯 **Real-world Applications** and practical use cases
- ✅ **Best Practices** for clustering implementation
- ⚠️ **Algorithm Comparisons** and method selection guidelines
- 📝 **Comprehensive Summaries** with key takeaways
- 🎨 **Custom Color Schemes** for enhanced visualization clarity

## Technical Requirements

- **Python 3.x** with data science libraries
- **Core Libraries**: NumPy, pandas, matplotlib, seaborn, scikit-learn, scipy
- **Specialized Libraries**: kneed (for elbow method optimization)
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Data Files**: Sample datasets included in `data/` folder (managed with DVC)
- **Themes**: Custom matplotlib themes in `themes/` folder (managed with DVC)

## Additional Resources

### Folders

- **`data/`**: Sample datasets used in the notebooks (DVC managed)
  - Social media and exercise data
  - Star Wars character dataset
  - Synthetic blob data generation parameters
- **`themes/`**: Custom matplotlib style themes for visualizations (DVC managed)
  - rose-pine.mplstyle for dendrogram visualizations

### Files

- **`data.dvc`**: Data Version Control file for dataset management
- **`themes.dvc`**: DVC file for theme resources
- **`.gitignore`**: Git ignore patterns for the lecture folder

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Fundamentals** (Ex 1-3): Build clustering foundation
   - K-Means from scratch → Optimal k selection → Real-world application

2. **Hierarchical Methods** (Ex 4-5): Explore tree-based clustering
   - Agglomerative clustering → Linkage method comparison

3. **Evaluation & Analysis** (Ex 6-8): Assess and interpret clusters
   - Silhouette scoring → WCSS evaluation → Feature analysis

4. **Density-Based Clustering** (Ex 9): Understand alternatives to partitioning methods
   - DBSCAN fundamentals → Comparison with K-Means → Handling arbitrary shapes

Each notebook builds upon concepts from previous ones, creating a comprehensive understanding of clustering algorithms and their practical applications in unsupervised learning scenarios.

## Usage Instructions

1. **Setup Environment**: Ensure all required Python libraries are installed (NumPy, pandas, scikit-learn, scipy, seaborn, kneed)
2. **Launch Notebooks**: Open notebooks in Jupyter or VS Code
3. **Follow Sequence**: Work through notebooks in the recommended order
4. **Run Examples**: Execute code cells to see clustering algorithms in action
5. **Experiment**: Modify parameters (k values, linkage methods, distance metrics) to understand their impact

This comprehensive collection provides both theoretical understanding and practical skills for implementing and evaluating clustering algorithms in real-world data mining and machine learning applications.
