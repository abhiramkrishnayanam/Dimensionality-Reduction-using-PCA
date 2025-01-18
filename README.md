# Dimensionality Reduction using Principal Component Analysis (PCA) 

## Overview

This project demonstrates the application of **Principal Component Analysis (PCA)** for dimensionality reduction. PCA is a powerful technique that transforms high-dimensional data into a smaller number of uncorrelated variables called principal components, while preserving as much variance in the dataset as possible.

---

## Dataset Details

### Iris Dataset
The **Iris dataset** is a classic dataset in machine learning and statistics. It contains 150 samples of iris flowers from three species (**Setosa**, **Versicolor**, and **Virginica**). The dataset is widely used for classification tasks but is also suitable for dimensionality reduction.

### Features:
The dataset contains the following features:
- **Sepal Length** (in cm)
- **Sepal Width** (in cm)
- **Petal Length** (in cm)
- **Petal Width** (in cm)

### Target:
- The target variable specifies the species of the iris flower:
  - **0**: Setosa
  - **1**: Versicolor
  - **2**: Virginica

---

## Key Steps Performed

1. **Data Standardization**:
   - Standardized the dataset to ensure all features have a mean of 0 and standard deviation of 1. This is a crucial step in PCA to eliminate the influence of feature scale.

2. **PCA Implementation**:
   - PCA was applied to the standardized dataset (excluding the target variable) to compute:
     - Principal components.
     - Explained variance for each component.
     - Cumulative explained variance.

3. **Cumulative Explained Variance Plot**:
   - A plot was generated to visualize the cumulative explained variance as a function of the number of principal components.
   - This plot helps determine the minimum number of components required to capture the desired level of variance.

---

## Understanding the Cumulative Explained Variance Plot

- **X-Axis**: The number of principal components.
- **Y-Axis**: The cumulative proportion of the variance explained by the selected components.
- **Interpretation**:
  - The plot showed that **95% of the variance** could be retained using the **first 2 principal components**.
  - This indicates that the dimensionality of the Iris dataset can be reduced from 4 features to 2, simplifying analysis and visualization.

---

## Key Insights

- PCA successfully reduced the dimensionality of the Iris dataset while retaining most of the variance.
- Based on the plot:
  - **95% of the variance** can be captured using just **2 principal components**.
  - This reduction allows for effective 2D visualization of the data.

---

## Benefits of This Work

- **Dimensionality Reduction**:
  - Reducing the dataset to 2 components simplifies visualization and improves computational efficiency.
- **Visualization**:
  - PCA enables high-dimensional data to be visualized effectively in 2D.
- **Feature Analysis**:
  - Highlights the underlying structure of the data and removes multicollinearity.

---

## Future Scope

- Visualize the first two principal components in a 2D scatter plot, colored by species.
- Use PCA-transformed data to train classification models and compare performance with the original dataset.
- Experiment with other dimensionality reduction techniques such as **t-SNE** or **UMAP**.

---

## Dependencies

- Python Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

---
