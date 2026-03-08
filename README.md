# Brain Tumor Detection using Support Vector Machines

## Overview

This project explores the application of **Machine Learning**, specifically **Support Vector Machines (SVM)**, for detecting brain tumors from MRI images.

The objective is to develop an automated classification system capable of distinguishing between **tumor** and **non-tumor** brain MRI images.

This work was conducted as part of a Bachelor's degree project in Computer Science.

---

## Dataset

The dataset used in this project is derived from the **BRATS 2015 challenge**.

Dataset characteristics:

* Total samples: 3762
* Classes:

  * Tumor
  * No Tumor
* Extracted features:

  * Mean
  * Variance
  * Standard deviation
  * Entropy
  * Contrast
  * Energy
  * Homogeneity

---

## Project Structure

```
brain-tumor-detection-svm
│
├── notebooks
│   ├── Datas_Preprocessing.ipynb
│   ├── SVM_Model.ipynb
│   └── SVM_Model_with_The_Same_Data_Train_Test.ipynb
│
├── images
│   └── confusion_matrix.png
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Workflow

### 1. Data Preprocessing

Steps include:

* checking missing values
* removing duplicates
* feature scaling using StandardScaler
* train/test split

Notebook:

```
Datas_Preprocessing.ipynb
```

---

### 2. Model Training

SVM classifiers were trained using different kernels:

* Linear
* Polynomial
* Radial Basis Function (RBF)
* Sigmoid

Hyperparameters were optimized using **GridSearchCV**.

Notebook:

```
SVM_Model.ipynb
```

---

### 3. Experimental Analysis

An experiment was conducted where training and testing were performed on the same dataset to illustrate potential overfitting effects.

Notebook:

```
SVM_Model_with_The_Same_Data_Train_Test.ipynb
```

---

## Results

The **RBF kernel** achieved the best performance:

* Accuracy: ~99%
* Balanced precision and recall
* Strong generalization with increasing dataset size

---

## Technologies Used

* Python
* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Author

Yasmine Rabiha OTMANI
Computer Science – Artificial Intelligence
