# Lecture #09 (Model Evaluation and Selection)

This folder contains the supporting material used during Lecture #08 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 29 October 2026**.

## Overview

This lecture covers how to measure the performance of a model honestly, how to compare candidate models, and how to choose the best one without fooling yourself. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and performance visualisations using scikit-learn. Every notebook relies exclusively on synthetic data and on the datasets bundled with scikit-learn, so no external download is required.

## Content Structure

### Evaluation Protocols

#### 1. **Holdout Evaluation** (`ex01_holdout_evaluation.ipynb`)

- **Learning Objectives**: Understanding the simplest evaluation protocol and its limitations
- **Techniques Covered**:
  - Single train/test split and its score
  - Repeating the split with many random seeds
  - Distribution, mean and standard deviation of the test accuracy
  - Why a single number can be misleading
- **Key Tools**: `train_test_split`, matplotlib histograms
- **Practical Applications**: Reporting results with an honest uncertainty estimate

#### 2. **Cross-Validation** (`ex02_cross_validation.ipynb`)

- **Learning Objectives**: Using all the data for both training and evaluation
- **Techniques Covered**:
  - `KFold`, `cross_val_score` and `cross_validate`
  - Multiple metrics in a single call
  - Visual diagram of the folds
  - Effect of `k` (2, 3, 5, 10, leave-one-out) on bias and variance
- **Key Tools**: `KFold`, `LeaveOneOut`, `cross_validate`
- **Practical Applications**: Small datasets, robust model comparison

#### 3. **Stratified Cross-Validation** (`ex03_stratified_cross_validation.ipynb`)

- **Learning Objectives**: Preserving the class distribution across folds
- **Techniques Covered**:
  - `StratifiedKFold` versus plain `KFold` on imbalanced data
  - Class proportions per fold
  - `RepeatedStratifiedKFold` and `GroupKFold`
- **Key Tools**: `StratifiedKFold`, `make_classification` with `weights`
- **Practical Applications**: Medical diagnosis, fraud detection, any rare-event problem

### Evaluation Metrics

#### 4. **Classification Metrics** (`ex04_classification_metrics.ipynb`)

- **Learning Objectives**: Computing and interpreting the standard classification measures
- **Techniques Covered**:
  - Confusion matrix and its four components
  - Accuracy, precision, recall, specificity, F1 and F-beta, by hand and with scikit-learn
  - Macro, micro and weighted averaging in the multiclass case
  - `classification_report` and confusion matrix heatmaps
- **Key Tools**: `confusion_matrix`, `classification_report`, `ConfusionMatrixDisplay`
- **Practical Applications**: Model reporting, threshold and cost analysis

#### 5. **Regression Metrics** (`ex05_regression_metrics.ipynb`)

- **Learning Objectives**: Measuring the quality of continuous predictions
- **Techniques Covered**:
  - MAE, MSE, RMSE, R² and MAPE
  - Residual plots and predicted-versus-actual plots
  - Sensitivity of MSE to a single outlier compared with MAE
- **Key Tools**: `mean_absolute_error`, `mean_squared_error`, `r2_score`
- **Practical Applications**: Forecasting, pricing, any numerical prediction task

### Threshold Analysis and Class Imbalance

#### 6. **ROC Curve and AUC** (`ex06_roc_curve_auc.ipynb`)

- **Learning Objectives**: Evaluating a classifier across all decision thresholds
- **Techniques Covered**:
  - ROC curves for several classifiers on the same problem
  - AUC and its probabilistic interpretation
  - Effect of moving the decision threshold on TPR and FPR
  - One-vs-rest ROC for multiclass problems
- **Key Tools**: `roc_curve`, `roc_auc_score`, `RocCurveDisplay`
- **Practical Applications**: Model selection independent of a fixed threshold

#### 7. **Precision-Recall and Class Imbalance** (`ex07_precision_recall_imbalance.ipynb`)

- **Learning Objectives**: Evaluating and training models when one class is rare
- **Techniques Covered**:
  - Precision-recall curve and average precision
  - ROC versus PR curve under strong imbalance
  - `class_weight="balanced"`, random over- and under-sampling
  - Threshold moving to maximise F1
- **Key Tools**: `precision_recall_curve`, `average_precision_score`, NumPy resampling
- **Practical Applications**: Fraud detection, rare disease screening, defect inspection

### Model Selection

#### 8. **Grid Search and Random Search** (`ex08_grid_and_random_search.ipynb`)

- **Learning Objectives**: Tuning hyperparameters without leaking the test set
- **Techniques Covered**:
  - `GridSearchCV` and `RandomizedSearchCV` on a `Pipeline`
  - Inspecting `cv_results_` as a DataFrame
  - Budget versus quality of the solution found
  - Heatmap of a two-dimensional grid
  - Nested cross-validation and the optimistic bias of non-nested scores
- **Key Tools**: `GridSearchCV`, `RandomizedSearchCV`, `cross_val_score`
- **Practical Applications**: Squeezing the last percent out of a model, fair comparisons

#### 9. **Learning and Validation Curves** (`ex09_learning_curves.ipynb`)

- **Learning Objectives**: Diagnosing what limits a model's performance
- **Techniques Covered**:
  - `learning_curve` with confidence bands
  - `validation_curve` over a regularisation parameter
  - Recognising high bias, high variance and a good fit
  - Deciding between more data and a different model
- **Key Tools**: `learning_curve`, `validation_curve`, matplotlib fill-between
- **Practical Applications**: Planning data collection, debugging underperforming models

#### 10. **Data Leakage and Reproducibility** (`ex10_leakage_and_reproducibility.ipynb`)

- **Learning Objectives**: Producing results that are both honest and repeatable
- **Techniques Covered**:
  - Preprocessing fitted before splitting and the inflated score it produces
  - Feature selection on noise features that fakes a high accuracy
  - The same procedure done correctly inside a `Pipeline`
  - Seeds, `random_state`, library versions and an evaluation checklist
- **Key Tools**: `Pipeline`, `SelectKBest`, `cross_val_score`
- **Practical Applications**: Peer review, reproducible research, production deployments

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each evaluation technique
- 🔍 **Step-by-step Explanations** with theoretical background
- 💻 **Hands-on Code Examples** with detailed comments
- 📊 **Interactive Visualizations** using matplotlib, seaborn and scikit-learn displays
- 📈 **Performance Analysis** with several complementary metrics
- 🎯 **Real-world Applications** and use case scenarios
- ✅ **Best Practices** for sound experimental protocols
- ⚠️ **Common Pitfalls** and how to avoid them
- 📝 **Comprehensive Summaries** with key takeaways

## Technical Requirements

- **Python 3.12** with the `damin2026` environment activated
- **Core Libraries**: NumPy, pandas, matplotlib, seaborn, scikit-learn
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Data Files**: None. All examples use synthetic data or datasets bundled with scikit-learn

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Protocols** (Ex 1-3): Holdout, cross-validation and stratification
2. **Metrics** (Ex 4-5): What to measure for classification and for regression
3. **Threshold Analysis** (Ex 6-7): ROC, AUC, precision-recall and class imbalance
4. **Selection** (Ex 8-9): Hyperparameter tuning, nested validation and learning curves
5. **Integrity** (Ex 10): Data leakage and reproducibility

Each notebook builds upon concepts from the previous ones and from Lecture #15 (Introduction to Machine Learning), forming a complete methodology for evaluating and selecting machine learning models.

## Usage Instructions

1. **Setup Environment**: Activate the `damin2026` Conda environment
2. **Launch Notebooks**: Open the notebooks in Jupyter or VS Code
3. **Follow Sequence**: Work through the notebooks in the recommended order
4. **Experiment**: Change the number of folds, the class balance and the search budget, and observe the effect
5. **Evaluate**: Always compare a tuned model against the baseline using the same protocol

This collection provides both the theoretical foundations and the practical skills required to evaluate models honestly and to select the best one for a real-world problem.
