# Housing Price Prediction with SVM and Dimensionality Reduction Techniques

This project uses various dimensionality reduction techniques to improve the accuracy of housing price prediction through Support Vector Machines (SVM).

---

## Overview

This project focuses on predicting housing prices based on various features, such as location and median income, using Support Vector Machines (SVM). The project explores several dimensionality reduction techniques, such as PCA, LDA, ICA, and FDA, to improve model performance and reduce computational complexity.

---

## Dataset

The dataset includes the following features:
- **Longitude & Latitude**
- **Housing median age**
- **Total rooms**
- **Total bedrooms**
- **Population**
- **Households**
- **Median income**
- **Ocean proximity**

**Target Variable:** Median house value.

---

## Model: Support Vector Machine (SVM)

SVM is a powerful supervised learning algorithm used for regression and classification tasks. For this project, SVM is employed to predict housing prices based on the input features.

### Kernel Selection
SVM models use different types of kernels, including:
- Linear Kernel
- Polynomial Kernel
- Radial Basis Function (RBF) Kernel

### Model Evaluation
- **Mean Squared Error (MSE):** Evaluates the model's performance.
- **Learning Curve:** Plots training vs. validation error across various training sizes.

#### SVM Evaluation Function
`evaluate_svm_kernels()` is used to evaluate the model with different kernels and compare their MSE on the test data.

---

## Dimensionality Reduction Techniques

To improve computational efficiency and potentially enhance performance, several dimensionality reduction techniques are applied:

### PCA (Principal Component Analysis)
- Reduces the dimensionality of the dataset while retaining as much variance as possible.
- **Visualization:** Explained variance ratio plot showcasing the variance retained by each component.

### LDA (Linear Discriminant Analysis)
- Maximizes separability between classes by reducing dimensionality.
- **Visualization:** Projection of the data to visualize target variable separation.

### ICA (Independent Component Analysis)
- Separates mixed signals into statistically independent components.
- **Visualization:** ICA component plots showing feature independence.

### LLE (Locally Linear Embedding)
- A non-linear technique preserving local neighborhood structure.
- **Visualization:** Scatter plot of LLE projections to examine local relationships.

### FDA (Fisher Discriminant Analysis)
- A supervised technique to maximize class separability by reducing dimensions.
- **Visualization:** FDA projections showing category predictions.

### MDA (Maximum Margin Discriminant Analysis)
- A variation of LDA focusing on maximizing margin between classes.

---

## Visualizations

1. **SVM Kernel Comparison:** Bar plot comparing MSE for each kernel.
2. **Learning Curves:** Training and validation errors plotted against training sizes.
3. **Decision Boundaries:** Visualized using the first two PCA components to understand SVM classification in lower dimensions.
4. **Dimensionality Reduction Comparison:** Bar plot comparing MSE of various techniques.

---

## Results

The project evaluates the impact of each dimensionality reduction technique on the SVM model's performance. Key takeaways:
- Techniques like PCA and LDA demonstrate notable performance improvements.
- A summary of results highlights the comparative effectiveness of PCA, ICA, and FDA based on MSE.

---

## Installation & Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/housing-price-prediction.git
   
   ---
   
2. Install required libraries:
    ```bash
   pip install -r requirements.txt
    
    ---
    
3. Run the Jupyter Notebook:
   
    ```bash
   jupyter notebook SVM_DR.ipynb

---

## Conclusion
This project demonstrates the effectiveness of combining SVM with dimensionality reduction techniques for housing price prediction. The results indicate that different dimensionality reduction methods impact model performance, with techniques like PCA and LDA showing notable improvements.
