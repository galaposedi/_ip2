# Activity Recognition using Machine Learning

## Overview

This project was developed as part of the **Data Mining 2** course. The objective is to recognize four different human activity 
states from physiological signals using machine learning techniques and data processing methods.

The project includes:

- data preprocessing
- dimensionality reduction
- visualization (PCA, UMAP, t-SNE)
- supervised classification
- unsupervised clustering
- association rule mining

The implementation is provided in a Jupyter Notebook (`IP2.ipynb`).

---

## Dataset

The project uses the **Activity Recognition from Physiological Signals** dataset.

Each observation belongs to one of four activity classes:

- Resting (1)
- Emotional activity (2)
- Mental activity (3)
- Physical activity (4)

The dataset contains physiological measurements obtained from:

- Electrocardiogram (ECG)
- Thoracic Bioimpedance (TEB)
- Electrodermal Activity (EDA)
- Other predictors made from these three (mean, median, sd, variance,...)

---

## Project Structure

```
IP2.ipynb
README.md
```

---

## Data Preprocessing

The preprocessing pipeline includes:

- loading raw data
- assigning feature names
- handling duplicate column names
- feature standardization
- feature selection using Pearson correlation
- Principal Component Analysis (PCA)

---

## Dimensionality Reduction

Two dimensionality reduction approaches were used:

- Pearson correlation filtering
- Principal Component Analysis (PCA)

For visualization purposes, **t-SNE** was applied after dimensionality reduction.

---

## Classification Models

The following supervised learning algorithms were evaluated:

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- AdaBoost
- XGBoost

Models were compared and briefly discussed using standard classification metrics.

---

## Clustering

Several clustering algorithms were applied and compared:

- K-Means++
- Agglomerative Clustering
- DBSCAN
- HDBSCAN
- OPTICS

Clustering quality was evaluated using:

- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Index

---

## Association Rule Mining

Association rules were generated after discretizing continuous variables.

Algorithms used:

- Apriori
- FP-Growth

The discovered rules were evaluated using common interestingness measures such as support, confidence, and lift.

---

## Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- mlxtend
- HDBSCAN

---

## Results

The notebook compares the performance of multiple classification and clustering algorithms on physiological signal data
and investigates relationships between features using association rule mining with visualisations and discussion of results.

---

## Author

**Gala Posedi**

Faculty of Mathematics, University of Belgrade

Course: Data Mining 2
