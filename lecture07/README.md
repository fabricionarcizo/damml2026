# Lecture #07 (Classification: Foundations)

This folder contains the supporting material used during Lecture #07 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 08 October 2026**.

## Overview

This lecture covers fundamental classification algorithms and evaluation metrics essential for supervised machine learning. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and performance visualizations using scikit-learn.

## Content Structure

### Core Classification Algorithms

#### 1. **k-Nearest Neighbors Classification** (`ex01_k_nearest_neighbors.ipynb`)

- **Learning Objectives**: Understanding distance-based classification and the k-NN algorithm
- **Techniques Covered**:
  - k-NN algorithm implementation
  - Distance metrics and neighbor selection
  - Hyperparameter tuning (k value selection)
  - Decision boundary visualization
- **Key Tools**: scikit-learn KNeighborsClassifier, matplotlib visualization
- **Practical Applications**: Pattern recognition, recommendation systems, image classification

#### 2. **Decision Tree Classification** (`ex02_decision_tree_sklearn.ipynb`)

- **Learning Objectives**: Understanding tree-based classification and decision-making processes
- **Techniques Covered**:
  - Decision tree construction and splitting criteria
  - Categorical feature encoding (LabelEncoder)
  - Tree visualization and interpretation
  - Model prediction and evaluation
- **Key Tools**: scikit-learn DecisionTreeClassifier, plot_tree visualization
- **Practical Applications**: Credit scoring, medical diagnosis, customer segmentation

#### 3. **Logistic Regression** (`ex03_logistic_regression.ipynb`)

- **Learning Objectives**: Understanding probabilistic classification and sigmoid functions
- **Techniques Covered**:
  - Logistic regression fundamentals
  - Sigmoid curve and decision boundaries
  - Probability prediction and interpretation
  - Binary classification with linear boundaries
- **Key Tools**: scikit-learn LogisticRegression, matplotlib curve plotting
- **Practical Applications**: Binary outcome prediction, risk assessment, medical screening

#### 4. **Naive Bayes Classification** (`ex04_naive_bayes.ipynb`)

- **Learning Objectives**: Understanding probabilistic classification with independence assumptions
- **Techniques Covered**:
  - Bayes' theorem application
  - Gaussian Naive Bayes implementation
  - Probability-based decision making
  - Model evaluation and visualization
- **Key Tools**: scikit-learn GaussianNB, matplotlib performance plotting
- **Practical Applications**: Text classification, spam filtering, document categorization

### Model Evaluation Metrics

#### 5. **Model Evaluation Metrics** (`ex05_model_evaluation.ipynb`)

- **Learning Objectives**: Understanding key classification performance measures
- **Techniques Covered**:
  - Accuracy, precision, recall, and F1-score calculations
  - Confusion matrix components
  - Metric interpretation and trade-offs
  - Performance assessment frameworks
- **Key Tools**: scikit-learn metrics functions
- **Practical Applications**: Model comparison, threshold optimization, performance reporting

#### 6. **Binary Confusion Matrix** (`ex06_binary_confusion_matrix.ipynb`)

- **Learning Objectives**: Visualizing and interpreting binary classification performance
- **Techniques Covered**:
  - Confusion matrix construction and annotation
  - True/False Positive/Negative analysis
  - Visual performance assessment
  - Decision tree evaluation example
- **Key Tools**: scikit-learn confusion_matrix, seaborn heatmap visualization
- **Practical Applications**: Diagnostic testing, quality control, binary classification evaluation

#### 7. **Multiclass Confusion Matrix** (`ex07_multiclass_confusion_matrix.ipynb`)

- **Learning Objectives**: Understanding multiclass classification evaluation
- **Techniques Covered**:
  - Multiclass confusion matrix interpretation
  - Class-wise performance analysis
  - Misclassification pattern identification
  - Multi-class decision tree evaluation
- **Key Tools**: scikit-learn ConfusionMatrixDisplay, matplotlib visualization
- **Practical Applications**: Multi-category classification, error analysis, model improvement

#### 8. **ROC Curve and AUC Analysis** (`ex08_roc_curve.ipynb`)

- **Learning Objectives**: Evaluating classifier performance across different thresholds
- **Techniques Covered**:
  - ROC curve construction and interpretation
  - Area Under the Curve (AUC) calculation
  - Multi-model performance comparison
  - Threshold-independent evaluation
- **Key Tools**: scikit-learn roc_curve, auc functions, matplotlib plotting
- **Practical Applications**: Model selection, threshold optimization, comparative analysis

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each classification technique
- 🔍 **Step-by-step Explanations** with theoretical background
- 💻 **Hands-on Code Examples** with detailed comments
- 📊 **Interactive Visualizations** using matplotlib, seaborn, and scikit-learn plotting
- 📈 **Performance Analysis** and evaluation metrics
- 🎯 **Real-world Applications** and use case scenarios
- ✅ **Best Practices** for algorithm selection and implementation
- ⚠️ **Common Pitfalls** and how to avoid them
- 📝 **Comprehensive Summaries** with key takeaways

## Technical Requirements

- **Python 3.x** with machine learning libraries
- **Core Libraries**: pandas, NumPy, matplotlib, seaborn, scikit-learn
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Data Files**: Sample datasets included in `exercises/` folder

## Additional Resources

### Folders

- **`exercises/`**: Practice exercises and supplementary datasets
  - `ex01_exercise_k_nearest_neighbors.py` through `ex08_exercise_roc_curve.py`: Corresponding exercises for each notebook
  - `original_penguins.csv`, `penguins_knn.csv`, `penguins_no_chinstraps.csv`: Palmer Penguins dataset variations for practice

### Files

- **`exercises.dvc`**: Data Version Control file for exercise materials
- **`.gitignore`**: Git ignore patterns for the lecture folder

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Algorithm Foundations** (Ex 1-4): Core classification algorithms

   - k-NN → Decision Trees → Logistic Regression → Naive Bayes

2. **Evaluation Methods** (Ex 5-8): Performance assessment techniques
   - Basic metrics → Binary confusion matrix → Multiclass evaluation → ROC analysis

Each notebook builds upon concepts from previous ones, creating a comprehensive understanding of classification algorithms and their evaluation essential for supervised machine learning applications.

## Usage Instructions

1. **Setup Environment**: Ensure all required Python libraries are installed
2. **Launch Notebooks**: Open notebooks in Jupyter or VS Code
3. **Follow Sequence**: Work through notebooks in the recommended order
4. **Practice**: Complete corresponding exercises in the `exercises/` folder
5. **Experiment**: Modify hyperparameters and compare model performance
6. **Evaluate**: Use evaluation metrics to assess and compare different approaches

This comprehensive collection provides both theoretical understanding and practical skills for effective classification and model evaluation in real-world machine learning applications.
