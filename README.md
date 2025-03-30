# Wisconsin-Breast-Cancer.
  The Wisconsin Breast Cancer Database contains data from 569 scans of cells from biopsied breast tissue.
  Image recognition was used to calculate features describing the shape and texture of cells in each image, such as cell radius, perimeter, and texture. 
  the database also includes whether the cell sample was benign or malignant. Since the correct cell type is known,classifying cells is a supervised learning task. 
  In the breast cancer dataset, malignant cells are labeled Diagnosis=1. Benign cells are labeled Diagnosis=0.

# Dataset

  It includes features computed from digitized images of a fine needle aspirate (FNA) of breast masses.
  Rows: 569
  Columns: 32
  Missing Values: None

# 📌 Key Features:
  ID: Patient identifier (not used in modeling)
  Diagnosis: Target label (M = malignant, B = benign)
  Radius mean, Texture mean, Area mean, etc.: Mean values of various cell characteristics
  Worst values: Features like Radius worst, Perimeter worst, etc., indicating extreme values
  Compactness, Concavity, Symmetry, and more describe cell shape and texture

Each feature helps build predictive models for cancer classification using supervised learning.

# Data Processing and Modeling Workflow
  Load and Clean the Data
  Import the dataset from a CSV file.
  Drop missing values using dropna().
  Encode Target Labels
    M (malignant) → 1
    B (benign) → 0

# Explore and Visualize Data
  Boxplots and scatter plots used to understand the distribution and relationships of features by diagnosis category.

# Select Features
  Input features like 'Radius mean', 'Texture mean' are selected.
  Target is the Diagnosis.

# Split Dataset
  Use train_test_split() with a random seed to split into training and testing sets.
  Apply StandardScaler to normalize feature values.

# Apply Machine Learning Models
  K-Nearest Neighbors (KNN)
  support Vector Machine (SVM)

# Evaluate Model Performance
  Metrics used: Accuracy , Precision , Recall ,Confusion Matrix

