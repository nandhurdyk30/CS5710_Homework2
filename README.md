# CS5710_Homework2

**Student Name:** Nandini Reddy  
**Course:** CS5710 Machine Learning  
**Semester:** Spring 2026  

---

## Assignment Overview

This homework focuses on implementing Linear Regression using two distinct techniques:

1. Analytical solution using the Normal Equation  
2. Iterative optimization using Gradient Descent built from scratch  

The purpose of the exercise is to compare the parameter estimates from both approaches and study how Gradient Descent converges during training.

---

## Dataset Description

A synthetic dataset was created using the following linear relationship:

**y = 3 + 4x + noise**

where:

- The feature \(x\) is sampled between 0 and 5  
- Noise is drawn from a Gaussian distribution  
- Number of observations: 200  

To enable learning of the intercept term, a column of ones was appended to the design matrix before model training.

---

## Normal Equation Method

The optimal parameters were computed directly using the matrix expression:

**θ = (XᵀX)⁻¹Xᵀy**

This approach produces the exact solution that minimizes the squared error.  
The resulting regression line is displayed along with the original data points.

---

## Gradient Descent Method

The same model was trained using iterative updates with the following configuration:

- Starting weights initialized to zero  
- Learning rate set to 0.05  
- Total iterations: 1000  
- Optimization objective: Mean Squared Error  

A training loss curve is included to illustrate how the error decreases as the parameters update.

---

## Visualizations Included

The notebook provides several plots to support analysis:

- Scatter plot of generated data  
- Regression fit using the Normal Equation  
- Regression fit using Gradient Descent  
- Overlay comparison of both fitted models  
- Graph of loss values across iterations  

---

## Findings

- The parameters obtained from Gradient Descent closely match those from the analytical solution.  
- The loss curve steadily decreases and stabilizes, indicating successful convergence.  
- Both models yield almost identical fitted lines, validating the correctness of the implementation.

---

## Code Notes

The notebook includes comments explaining:

- How the dataset is generated  
- The mathematical steps used in each method  
- The update rules for Gradient Descent  
- The plotting process  

These notes help ensure the workflow is easy to follow and reproduce.

---

## Summary

This assignment highlights the connection between closed-form optimization and iterative learning methods. It demonstrates how Gradient Descent can approximate the analytical Linear Regression solution while providing insight into the training dynamics.
