# 1.3 Supervised Learning: Regression

## Notation to Remember
- **R**: Real numbers
- **R^d**: d-dimensional vector of real numbers
- \((x_1)^2\): Square of the first coordinate of the vector \(x\)
- **Mode of \(x\)**: Length of \(x\)
- \(1(2 \text{ is even}) = 1\), \(1(2 \text{ is odd}) = 0\)
for example 1(355 % 2 = 1) this tends to odd outcome should be 0
            1(786 % 2 = 0) this tends to even outcome should be 1


## Overview
Supervised learning involves **curve fitting**, which is similar to what you might have done in school by joining points on a graph. This encompasses both regression and classification learning.

### Types of Learning
- **Supervised Learning**:
  - **Regression**: Predicting continuous outcomes.
  - **Classification**: Predicting discrete labels.

- **Unsupervised Learning**:
  - **Dimensionality Reduction**: Reducing the number of features while retaining important information.
  - **Density Estimation**: Estimating the distribution of data points in a dataset.

## Example of Regression
### Predicting House Prices
We aim to predict house prices based on the following features:
- Number of Rooms
- Area (in square feet)
- Distance from the city center (in miles)

The data values are represented in the form of tuples \((x_i, y_i)\), where:
- \(x_i\) is a vector of features \([\text{rooms}, \text{area}, \text{distance}]\)
- \(y_i\) is the corresponding house price.

### Loss Function
To evaluate our predictions, we consider the function \(f(x_i)\) which represents our model's predicted price for features \(x_i\). The loss can be captured using the squared difference:

Classification modal = L = (f(x_i) != y_i)
\[
Regression modal L = (f(x_i) - y_i)^2
\]

This loss function quantifies how far \(f(x_i)\) is from \(y_i\). The goal is to minimize this loss, ensuring that:
- \(f(x_i)\) is not too much above \(y_i\)
- \(f(x_i)\) is not too much below \(y_i\)

By minimizing the loss, we aim to fit our model as closely as possible to the actual data points.
