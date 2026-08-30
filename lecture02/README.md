# Lecture #02 (Introduction to Machine Learning)

This folder contains the supporting material used during **Lecture #02** of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 03 September 2026**.

## Overview

This lecture introduces the vocabulary, the workflow and the mental models required to do machine learning properly. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and visualisations using scikit-learn. Every notebook relies exclusively on synthetic data and on the datasets bundled with scikit-learn, so no external download is required.

## Content Structure

### Concepts and Terminology

#### 1. **Machine Learning Terminology** (`ex01_ml_terminology.ipynb`)

- **Learning Objectives**: Speaking the language of machine learning with precision
- **Techniques Covered**:
  - Instances, attributes, features and targets
  - The data matrix `X` and the target vector `y`
  - Models, parameters and hyperparameters
  - Inspecting a dataset with pandas
- **Key Tools**: scikit-learn `load_iris`, pandas DataFrame inspection
- **Practical Applications**: Reading any dataset description and identifying what can be predicted

#### 2. **Types of Learning** (`ex02_types_of_learning.ipynb`)

- **Learning Objectives**: Recognising which learning paradigm a problem belongs to
- **Techniques Covered**:
  - Supervised classification and supervised regression
  - Unsupervised clustering and dimensionality reduction
  - Comparing the four paradigms on comparable data
- **Key Tools**: `make_classification`, `make_regression`, `make_blobs`, `KMeans`, `PCA`
- **Practical Applications**: Problem framing, choosing an algorithm family

#### 3. **Features and Targets** (`ex03_features_and_targets.ipynb`)

- **Learning Objectives**: Turning raw records into a numerical feature matrix
- **Techniques Covered**:
  - Numerical, nominal and ordinal features
  - One-hot and ordinal encoding
  - Standardisation and `ColumnTransformer`
  - Inspecting the generated feature names
- **Key Tools**: `OneHotEncoder`, `OrdinalEncoder`, `StandardScaler`, `ColumnTransformer`
- **Practical Applications**: Preparing heterogeneous tabular data for any estimator

### The Estimator API

#### 4. **Your First Scikit-learn Model** (`ex04_first_sklearn_model.ipynb`)

- **Learning Objectives**: Mastering the four verbs of the scikit-learn API
- **Techniques Covered**:
  - `fit`, `predict`, `predict_proba` and `score`
  - Fitted attributes ending with an underscore
  - Swapping estimators without changing the surrounding code
  - Decision boundary visualisation
- **Key Tools**: `KNeighborsClassifier`, `LogisticRegression`, matplotlib
- **Practical Applications**: Rapid prototyping and model comparison

#### 5. **Training and Inference** (`ex05_training_and_inference.ipynb`)

- **Learning Objectives**: Separating the training phase from the prediction phase
- **Techniques Covered**:
  - Predicting on new, unseen instances
  - Hard predictions versus probabilities and thresholding
  - Persisting and reloading a fitted model
  - Why a transformer must never be re-fitted at inference time
- **Key Tools**: `joblib`, `predict_proba`, `StandardScaler`
- **Practical Applications**: Deployment, batch scoring, model serving

### Datasets and Generalization

#### 6. **Training, Validation and Test Sets** (`ex06_train_validation_test.ipynb`)

- **Learning Objectives**: Building an honest evaluation protocol
- **Techniques Covered**:
  - Three-way splitting with two calls to `train_test_split`
  - Stratification and class proportions per split
  - Using the validation set to select a hyperparameter
  - Opening the test set exactly once
- **Key Tools**: `train_test_split`, pandas summary tables
- **Practical Applications**: Any supervised project, mandatory assignment reporting

#### 7. **The Generalization Gap** (`ex07_generalization_gap.ipynb`)

- **Learning Objectives**: Measuring the distance between training and test performance
- **Techniques Covered**:
  - Error as a function of the training-set size
  - Error as a function of model complexity
  - Visualising and interpreting the gap
- **Key Tools**: `DecisionTreeClassifier`, `load_breast_cancer`, matplotlib
- **Practical Applications**: Deciding whether to collect more data or change the model

#### 8. **Overfitting and Underfitting** (`ex08_overfitting_underfitting.ipynb`)

- **Learning Objectives**: Diagnosing the two failure modes of a model
- **Techniques Covered**:
  - Polynomial regression of increasing degree on a noisy sine wave
  - Train and test RMSE side by side
  - The U-shaped error curve
- **Key Tools**: `PolynomialFeatures`, `LinearRegression`, `make_pipeline`
- **Practical Applications**: Model complexity selection, regularisation decisions

#### 9. **The Bias-Variance Trade-off** (`ex09_bias_variance_tradeoff.ipynb`)

- **Learning Objectives**: Decomposing the prediction error into its components
- **Techniques Covered**:
  - Monte-Carlo simulation over many resampled training sets
  - Estimating bias squared, variance and total error
  - Visualising the instability of high-complexity models
- **Key Tools**: NumPy simulation, `PolynomialFeatures`, matplotlib
- **Practical Applications**: Explaining why ensembles and regularisation work

### Baselines and Pipelines

#### 10. **Baseline Models and Pipelines** (`ex10_baseline_and_pipeline.ipynb`)

- **Learning Objectives**: Establishing a reference point and a leakage-free workflow
- **Techniques Covered**:
  - `DummyClassifier` strategies on imbalanced data
  - Why accuracy alone is misleading
  - `DummyRegressor` for regression problems
  - End-to-end `Pipeline` with preprocessing and estimator
- **Key Tools**: `DummyClassifier`, `DummyRegressor`, `Pipeline`, `ColumnTransformer`
- **Practical Applications**: Sanity checking every experiment before scaling it up

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each concept
- 🔍 **Step-by-step Explanations** with theoretical background
- 💻 **Hands-on Code Examples** with detailed comments
- 📊 **Visualizations** using matplotlib and scikit-learn plotting utilities
- 📈 **Performance Analysis** of the trained models
- 🎯 **Real-world Applications** and use case scenarios
- ✅ **Best Practices** for building honest machine learning experiments
- ⚠️ **Common Pitfalls** and how to avoid them
- 📝 **Comprehensive Summaries** with key takeaways

## Technical Requirements

- **Python 3.12** with the `damml2026` environment activated
- **Core Libraries**: NumPy, pandas, matplotlib, seaborn, scikit-learn
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Data Files**: None. All examples use synthetic data or datasets bundled with scikit-learn

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Vocabulary and Framing** (Ex 1-3): Terminology, learning paradigms and feature construction
2. **The Estimator API** (Ex 4-5): Training a model and using it for inference
3. **Honest Evaluation** (Ex 6-7): Data splitting and the generalization gap
4. **Model Complexity** (Ex 8-9): Overfitting, underfitting, bias and variance
5. **Good Practice** (Ex 10): Baselines and pipelines

## Usage Instructions

1. **Setup Environment**: Activate the `damml2026` Conda environment
2. **Launch Notebooks**: Open the notebooks in Jupyter or VS Code
3. **Follow Sequence**: Work through the notebooks in the recommended order
4. **Experiment**: Change the seeds, the model complexity and the split sizes, and observe the effect
5. **Reflect**: Compare every result against the baseline before drawing conclusions

This collection provides both the theoretical vocabulary and the practical skills needed to start any supervised machine learning project with a sound methodology.
