# Lecture #08 (Classification: Advanced Techniques)

This folder contains the supporting material used during Lecture #08 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 22 October 2026**.

## Overview

This lecture covers advanced classification techniques in machine learning, focusing on Support Vector Machines (SVM) and Neural Networks. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and comprehensive visualizations demonstrating both theoretical concepts and practical applications.

## Content Structure

### Support Vector Machine Fundamentals

#### 1. **Decision Boundary Exploration** (`ex01_several_decision_boundaries.ipynb`)

- **Learning Objectives**: Understanding multiple possible decision boundaries and the need for optimal selection
- **Techniques Covered**:
  - Logistic regression with decision boundaries
  - Random noise impact on boundary placement
  - Multiple solution visualization
  - Decision boundary stability analysis
- **Key Tools**: scikit-learn LogisticRegression, NumPy, matplotlib
- **Practical Applications**: Binary classification scenarios, classifier comparison, boundary uncertainty

#### 2. **Margin Maximization Concept** (`ex02_maximizing_margin.ipynb`)

- **Learning Objectives**: Understanding the fundamental principle of SVM margin maximization
- **Techniques Covered**:
  - Support vector identification
  - Margin calculation and visualization
  - Hyperplane comparison
  - Geometric interpretation of SVM optimization
- **Key Tools**: scikit-learn SVC, custom margin visualization functions
- **Practical Applications**: Optimal classifier selection, geometric machine learning understanding

#### 3. **Linear Support Vector Machine** (`ex03_support_vector_machine.ipynb`)

- **Learning Objectives**: Complete implementation and visualization of linear SVM
- **Techniques Covered**:
  - Linear SVM with hard margin
  - Support vector identification
  - Decision boundary and margin visualization
  - Mathematical foundation demonstration
- **Key Tools**: scikit-learn SVC with linear kernel, matplotlib annotations
- **Practical Applications**: Linearly separable data classification, SVM fundamentals

#### 4. **Non-Linear SVM with Kernel Trick** (`ex04_non_linear_svm.ipynb`)

- **Learning Objectives**: Extending SVM to non-linearly separable data using kernel methods
- **Techniques Covered**:
  - RBF (Radial Basis Function) kernel
  - Kernel trick demonstration
  - 2D to 3D transformation visualization
  - Non-linear decision boundary mapping
- **Key Tools**: scikit-learn SVC with RBF kernel, 3D plotting, make_circles dataset
- **Practical Applications**: Complex pattern recognition, circular/non-linear data classification

#### 5. **Kernel Function Comparison** (`ex05_popular_kernels.ipynb`)

- **Learning Objectives**: Comparing different kernel functions and their decision boundaries
- **Techniques Covered**:
  - Polynomial kernel implementation
  - RBF kernel applications
  - Sigmoid kernel characteristics
  - Kernel selection strategies
- **Key Tools**: scikit-learn SVC with multiple kernels, subplot comparisons
- **Practical Applications**: Kernel selection for different data types, performance optimization

### Neural Network Architectures

#### 6. **Feedforward Neural Networks** (`ex06_handwriting_nn.ipynb`)

- **Learning Objectives**: Building and training deep neural networks for image classification
- **Techniques Covered**:
  - Multi-layer perceptron architecture
  - MNIST dataset preprocessing
  - Model compilation and training
  - Performance evaluation and visualization
  - ONNX model export
- **Key Tools**: TensorFlow/Keras, MNIST dataset, tf2onnx, model visualization
- **Practical Applications**: Handwritten digit recognition, image classification, model deployment

#### 7. **Convolutional Neural Networks** (`ex07_convolutional_neural_network.ipynb`)

- **Learning Objectives**: Understanding CNN architecture for improved image processing
- **Techniques Covered**:
  - Convolutional and pooling layers
  - CNN architecture design
  - QMNIST dataset handling
  - Model performance metrics
  - PyTorch implementation
- **Key Tools**: PyTorch, torchvision, QMNIST dataset, sklearn metrics, model graph visualization
- **Practical Applications**: Advanced image recognition, computer vision, feature extraction

### Time Series and Sequential Data

#### 8. **Real-Time Data Processing** (`ex08_time_series_example.py`)

- **Learning Objectives**: Real-time data capture and visualization techniques
- **Techniques Covered**:
  - MediaPipe hand tracking
  - Real-time plotting with pyqtgraph
  - Computer vision integration
  - Live data stream processing
- **Key Tools**: OpenCV, MediaPipe, pyqtgraph, real-time visualization
- **Practical Applications**: Motion tracking, real-time analytics, human-computer interaction

#### 9. **Recurrent Neural Networks** (`ex09_lstm_gru_models.ipynb`)

- **Learning Objectives**: Sequential data modeling with LSTM and GRU architectures
- **Techniques Covered**:
  - LSTM (Long Short-Term Memory) networks
  - GRU (Gated Recurrent Unit) networks
  - Time series prediction
  - PyTorch Lightning framework
  - Model comparison and evaluation
- **Key Tools**: PyTorch Lightning, custom dataset classes, time series generation
- **Practical Applications**: Sequential pattern recognition, time series forecasting, temporal data analysis

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each advanced technique
- 🔍 **Step-by-step Explanations** with mathematical foundations
- 💻 **Hands-on Code Examples** with detailed comments and best practices
- 📊 **Interactive Visualizations** using matplotlib, 3D plotting, and custom visualization functions
- 📈 **Performance Analysis** and model evaluation metrics
- 🎯 **Real-world Applications** and practical use case scenarios
- ✅ **Best Practices** for model selection and hyperparameter tuning
- ⚠️ **Common Pitfalls** and debugging strategies
- 📝 **Comprehensive Summaries** with implementation guidelines
- 🔧 **Model Export** and deployment preparation (ONNX format)

## Technical Requirements

- **Python 3.x** with machine learning and deep learning libraries
- **Core Libraries**: scikit-learn, NumPy, matplotlib, pandas
- **Deep Learning**: TensorFlow/Keras, PyTorch, PyTorch Lightning
- **Computer Vision**: OpenCV, MediaPipe (for real-time examples)
- **Visualization**: pyqtgraph, torchviz
- **Model Export**: tf2onnx, ONNX runtime
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Hardware**: GPU recommended for neural network training (optional)

## Additional Resources

### Folders

- **`data/`**: Training datasets including QMNIST (DVC managed)
- **`models/`**: Trained model files and architecture diagrams (DVC managed)
- **`lightning_logs/`**: PyTorch Lightning training logs and checkpoints

### Files

- **`data.dvc`**: Data Version Control file for dataset management
- **`models.dvc`**: DVC file for trained models and artifacts
- **`.gitignore`**: Git ignore patterns for the lecture folder

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **SVM Fundamentals** (Ex 1-3): Build foundation understanding

   - Decision boundaries → Margin concepts → Linear SVM implementation

2. **Advanced SVM** (Ex 4-5): Extend to complex scenarios

   - Non-linear kernels → Kernel comparison and selection

3. **Neural Network Basics** (Ex 6): Introduction to deep learning

   - Feedforward networks → MNIST classification

4. **Advanced Neural Networks** (Ex 7, 9): Specialized architectures

   - Convolutional networks → Recurrent networks

5. **Real-time Applications** (Ex 8): Practical implementation
   - Live data processing and visualization

Each notebook builds upon fundamental concepts while introducing increasingly sophisticated techniques for handling complex classification problems.

## Usage Instructions

1. **Setup Environment**: Install required Python libraries and frameworks
2. **Hardware Check**: Verify GPU availability for neural network training (optional)
3. **Launch Notebooks**: Open notebooks in Jupyter or VS Code
4. **Follow Sequence**: Work through notebooks in the recommended order
5. **Experiment**: Modify hyperparameters and architectures with your own data
6. **Deploy**: Practice model export and deployment techniques

This comprehensive collection bridges theoretical machine learning concepts with practical implementation skills, preparing students for real-world classification challenges in data mining and machine learning applications.
