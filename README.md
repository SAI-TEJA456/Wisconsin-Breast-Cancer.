# Wisconsin-Breast-Cancer.

The Wisconsin Breast Cancer Database contains data from 569 scans of cells from biopsied breast tissue. Image recognition was used to calculate features describing the shape and texture of cells in each image, such as cell radius, perimeter, and texture. The database also includes whether the cell sample was benign or malignant. Since the correct cell type is known, classifying cells is a supervised learning task. In the breast cancer dataset, malignant cells are labeled Diagnosis=1. Benign cells are labeled Diagnosis=0.

# Supervised Learning on Cancer Dataset**
This repository contains a series of Jupyter notebooks designed to guide students through a hands-on learning experience with supervised machine learning techniques applied to a cancer dataset.

📁 Notebooks Overview
Notebook	Description
SupervisedLearning_Cancer_01.ipynb	Notebook 1 sets the stage, likely focusing on initial data exploration, preprocessing, and understanding the structure of the dataset. (No description markdown found)
SupervisedLearning_Cancer_02.ipynb	Introduces participation activities involving supervised learning, with notes that results may vary due to randomization. Analyses should be performed using seed=123.
SupervisedLearning_Cancer_03.ipynb	Continues the analysis with more participation activities. Emphasizes reproducibility with the specified seed.
SupervisedLearning_Cancer_04.ipynb	Final steps of the supervised learning workflow, continuing with the same randomization considerations as earlier notebooks.

🎯 Objective
The goal of this series is to apply supervised learning algorithms to a real-world medical dataset, specifically focusing on cancer prediction. The notebooks include exercises that reinforce machine learning concepts and encourage experimentation.

🛠 Technologies Used
Python 3.x
Jupyter Notebook
Scikit-learn
Pandas
Matplotlib / Seaborn

 Data Processing and Modeling Workflow
Load and Clean the Data

Import the dataset from a CSV file.

Drop missing values using dropna().

Encode Target Labels

Convert diagnosis values:

M (malignant) → 1

B (benign) → 0

Explore and Visualize Data

Boxplots and scatter plots used to understand the distribution and relationships of features by diagnosis category.

Select Features

Input features like 'Radius mean', 'Texture mean' are selected.

Target is the Diagnosis.

Split Dataset

Use train_test_split() with a random seed to split into training and testing sets.

Standardize Features

Apply StandardScaler to normalize feature values.

Apply Machine Learning Models

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Evaluate Model Performance

Metrics used:

Accuracy

Precision

Recall

Confusion Matrix

