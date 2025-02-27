# Machine Learning - Lasso Regression Proof of Concept (POC)

This repository demonstrates how **Lasso Regression** helps in feature selection by automatically removing irrelevant variables. The examples focus on two real-world scenarios:

1. **Real Estate Price Prediction**: Estimating property prices while eliminating unimportant features.
2. **Disease Diagnosis**: Predicting disease risk by selecting only the most relevant medical factors.

## What is Lasso Regression?

**Lasso Regression** (Least Absolute Shrinkage and Selection Operator) is a regression technique that:
- **Selects the most relevant features** by reducing the impact of less important ones.
- **Removes irrelevant variables** by setting their coefficients to zero.
- **Prevents overfitting**, making the model simpler and more efficient.

### Why Use Lasso Regression?
- **Reduces complexity** by automatically eliminating unnecessary variables.
- **Improves model accuracy** by keeping only the most important features.
- **Avoids overfitting**, making predictions more reliable.

---

## Running on Google Colab

### Step 1: Open the Notebooks in Colab
Click the links below to open the examples directly in **Google Colab**:
- [Real Estate Price Prediction](https://colab.research.google.com/github/your-repo/real_estate_lasso.ipynb)
- [Disease Diagnosis](https://colab.research.google.com/github/your-repo/disease_diagnosis_lasso.ipynb)

### Step 2: Install Dependencies (if needed)
Google Colab usually comes with the required libraries pre-installed. However, if needed, run:
```python
!pip install numpy matplotlib scikit-learn pandas
```

### Step 3: Run the Cells
Each notebook contains explanations, data, and visualizations. Execute the cells in order to train the models and visualize results.

---

## Example 1: Real Estate Price Prediction

This model predicts **property prices** based on various features, while **automatically removing irrelevant ones**:

- **Input Features**: 
  - Property size (m²)
  - Number of rooms
  - Year of construction
  - Distance from the city center
  - Wall color (irrelevant)
  - Door handle type (irrelevant)
- **Output**: Predicted property price
- **Comparison**: Standard Linear Regression vs. Lasso Regression

### Notebook Highlights:
- **Linear Regression model** considers all variables, even those that don’t impact price.
- **Lasso Regression removes unnecessary variables**, simplifying the model.
- **The model focuses only on relevant factors**, improving efficiency.

---

## Example 2: Disease Diagnosis

This model predicts **disease risk** based on various health indicators, while **automatically selecting only the important ones**:

- **Input Features**:
  - Age
  - Weight
  - Blood pressure
  - Family history
  - Blood type (irrelevant)
  - Eye color (irrelevant)
- **Output**: Predicted disease risk score
- **Comparison**: Standard Linear Regression vs. Lasso Regression

### Notebook Highlights:
- **Linear Regression includes all factors**, even those that don’t affect health.
- **Lasso Regression removes irrelevant medical features**, such as **eye color and blood type**.
- **The model keeps only significant health indicators**, ensuring a more precise diagnosis.

---

## Visualizing Results

Each notebook generates a **scatter plot** comparing **Linear Regression vs. Lasso Regression**:
- **Blue dots**: Predictions using Linear Regression.
- **Red dots**: Predictions using Lasso Regression.
- **Dashed black line**: Ideal fit (perfect prediction).
- **Lower MSE in Lasso Regression**: Demonstrates improved model efficiency.

---

## Conclusion

**Lasso Regression** is a powerful feature selection technique that **removes unnecessary variables**, leading to more efficient and accurate models. It is widely used in:
- **Real estate pricing**
- **Medical diagnostics**
- **Finance and predictive modeling**

By using **Lasso Regression**, we ensure that:
- The model remains **simple and efficient**.
- The most **important features are selected**.
- Predictions are **more reliable** for real-world applications.

## License

This project is released under the MIT License.
