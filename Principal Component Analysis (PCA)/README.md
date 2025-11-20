# 📉 Analysis: Principal Component Analysis (PCA)

[View the Notebook: Principal Component Analysis (PCA).ipynb](./Principal%20Component%20Analysis%20(PCA).ipynb)

## Project Focus
The goal of this analysis was to implement dimensionality reduction techniques to simplify complex datasets while retaining essential information.

* **Perform PCA** to reduce the number of features in a dataset.
* **Evaluate Explained Variance** to determine the appropriate number of principal components to retain.
* **Handle Non-Linear Data** using Kernel PCA methods.
* **Maximize Class Separability** using Linear Discriminant Analysis (LDA) for supervised dimensionality reduction.

---

## 📝 Analysis Content Summary

The notebook covers three distinct approaches to feature reduction:

### 1. Standard Principal Component Analysis (PCA)
* **Standardization:** Applied `StandardScaler` to normalize the feature set before analysis.
* **Variance Retention:** Configured PCA to retain 99% of the variance, automatically selecting the necessary number of components (reducing 11 features to 10 in the example).

### 2. Kernel PCA for Linearly Inseparable Data
* **Non-Linear Transformation:** Used `KernelPCA` with an "rbf" (Radial Basis Function) kernel to project data into a higher-dimensional space where it becomes linearly separable.
* **Dimensionality Reduction:** Reduced specific numerical features (e.g., 'alcohol', 'pH') down to a single component.

### 3. Linear Discriminant Analysis (LDA)
* **Supervised Reduction:** Unlike standard PCA, LDA uses the target variable ('quality') to find component axes that maximize the separation between classes.
* **Efficiency:** Demonstrated extreme reduction (from 11 features to 1) while maintaining significant class discriminatory power.

---

## 📂 Data Files Used

* **Dataset:** `winequality-red.csv`
