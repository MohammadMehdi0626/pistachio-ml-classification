# Pistachio ML Classification

## Project Overview

This project focuses on applying and comparing different machine learning
classification algorithms for pistachio classification.

The project covers the complete machine learning workflow, including:

- Data preprocessing
- Exploratory data analysis (EDA)
- Feature preparation
- Training multiple classification models
- Model evaluation
- Comparison of classification performance

The following machine learning models were investigated:

- SGDClassifier
- Logistic Regression
- Multi-Layer Perceptron (MLP)
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Decision Tree

## Dataset

The project uses a pistachio dataset for binary classification.

The final evaluation was performed on a test set containing:

- **430 samples**
- **29 features**

The dataset was prepared and processed before being used for training and
evaluation of the machine learning models.

## Data Preprocessing

The preprocessing pipeline was performed separately for the training,
validation, and test datasets.

The main preprocessing steps included:

- Missing-value analysis
- Target-label encoding
- Outlier analysis and treatment
- Feature and data reduction
- Feature transformation
- Min-Max normalization
- Standardization

Both normalized and standardized versions of the processed data were
prepared for subsequent machine learning experiments.

## Exploratory Data Analysis

Exploratory data analysis was performed to understand the structure,
distribution, and relationships within the dataset.

The analysis included:

- Feature distribution analysis
- Histogram and boxplot visualization
- Pairwise feature relationship analysis
- Multivariate visualization
- Outlier investigation
- Examination of feature behavior across the target classes

## Machine Learning Models

Several classification algorithms were implemented and evaluated as part
of the project.

### SGDClassifier

A linear classification model based on stochastic gradient descent.

### Logistic Regression

A linear classification algorithm used as a classification model.

### Multi-Layer Perceptron (MLP)

A neural-network-based classifier used to investigate nonlinear
relationships between the input features and the target variable.

### Support Vector Machine (SVM)

Several SVM configurations were investigated, including:

- Linear SVM
- Polynomial SVM
- NuSVC

### K-Nearest Neighbors (KNN)

A distance-based classification algorithm evaluated using the processed
feature set.

### Decision Tree

A tree-based classification model used to investigate rule-based
partitioning of the feature space.

## Model Evaluation

The trained models were evaluated on the test dataset using multiple
classification metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Specificity

Using multiple evaluation metrics provides a broader view of model
classification performance rather than relying on accuracy alone.

## Results

The final models were evaluated on the test set.

| Model | Accuracy | Precision | Recall | F1-score | Specificity |
|---|---:|---:|---:|---:|---:|
| SGDClassifier | 94.88% | 90.45% | 98.36% | 94.24% | 92.31% |
| Logistic Regression | 100% | 100% | 100% | 100% | 100% |
| MLP | 99.77% | 99.46% | 100% | 99.73% | 99.60% |
| KNN | 100% | 100% | 100% | 100% | 100% |
| Linear SVM | 98.84% | 97.85% | 99.45% | 98.64% | 98.38% |
| Polynomial SVM | 100% | 100% | 100% | 100% | 100% |
| NuSVC | 100% | 100% | 100% | 100% | 100% |
| Decision Tree | 100% | 100% | 100% | 100% | 100% |

## Project Structure

```text
pistachio-ml-classification/
│
├── notebooks/
│   ├── 01_Preprocessing_EDA.ipynb
│   ├── 02_SGDClassifier.ipynb
│   ├── 03_Logistic_Regression.ipynb
│   ├── 04_MLP.ipynb
│   ├── 05_SVM.ipynb
│   ├── 06_KNN.ipynb
│   ├── 07_Decision_Tree.ipynb
│   └── 08_Final_Evaluation.ipynb
│
├── models/
├── .gitignore
├── requirements.txt
└── README.md