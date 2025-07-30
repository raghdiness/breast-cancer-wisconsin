
# SVM Classifier – Breast Cancer Wisconsin Diagnostic Dataset

This project applies a Support Vector Machine (SVM) model to classify breast tumors as benign or malignant using the Breast Cancer Wisconsin Diagnostic dataset from the UCI Machine Learning Repository.

## Overview

The dataset contains measurements from digitized images of fine needle aspirate (FNA) of breast masses. The goal is to predict whether a tumor is benign or malignant based on features like radius, texture, perimeter, and more.

## Dataset Source

[UCI Machine Learning Repository – Breast Cancer Wisconsin (Diagnostic) Data Set](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))

- Instances: 569
- Features: 30 (mean, standard error, and worst value for 10 properties)
- Target: Diagnosis (M = malignant, B = benign)

## Workflow

1. **Data Loading**
   - Data is fetched directly from the UCI repository.
   - Columns are renamed for readability based on dataset documentation.

2. **Preprocessing**
   - ID column is dropped.
   - Diagnosis column is label-encoded (M = 1, B = 0).
   - All features are standardized using `StandardScaler`.

3. **Exploratory Data Analysis**
   - Correlation matrix is plotted to visualize relationships.
   - Optional: Pair plots and feature selection can be added.

4. **Train/Test Split**
   - The dataset is split into training and test sets (usually 80/20).

5. **Modeling**
   - SVM is trained using:
     - Linear kernel
     - Polynomial kernel
     - RBF (Gaussian) kernel
   - Model accuracy is evaluated on both training and test sets.

6. **Results**
   - Accuracy for each kernel is reported and compared.
   - Best-performing kernel is identified.

## Libraries Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## Skills Demonstrated

- Data preprocessing
- Feature scaling
- Label encoding
- Correlation analysis
- SVM classification with different kernels
- Model evaluation and comparison

## How to Run

1. Clone or download this repository.
2. Open the notebook `SVM Assignment_Raghda Haikal.ipynb` in Jupyter or Google Colab.
3. Run all cells to execute the full pipeline.
4. You can tweak kernel parameters to experiment with different SVM settings.

## Author

Raghda Haikal  
Machine Learning Assignment – SVM Classifier  
Instructor: *[Add your instructor's name if required]*

---

