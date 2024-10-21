# Notes on Clustering and Kernel Functions

## 1. K-Means Clustering with K=3
- **Data Points**: 
  - (2, 2), (3, 3), (4, 4), (10, 10), (12, 12), (13, 13)
- **Initial Centroid**: (2, 2)
- **Final Centroids** (after applying K-Means++):
  - Cluster 1: Points near (2, 2)
  - Cluster 2: Points around (10, 10)
  - Cluster 3: Points around (12, 12)

## 2. PCA and Eigenvalues
- **Dataset**: 50 points in \( \mathbb{R}^5 \)
- **Eigenvalues**: 
  - 1.7, 1.4, 0.25, 0.20, 0.005
- **Principal Components**: 
  - To retain at least 95% of the variance, a good choice is \( k = 2 \) (sum of the top two eigenvalues).

## 3. Manhattan Distance
- **Definition**: The Manhattan distance between two points \( \mathbf{p} \) and \( \mathbf{q} \) is given by:
  \[
  D = \sum_{i=1}^{n} |p_i - q_i|
  \]

## 4. Closest Cluster Mean for New Point
- **Cluster Means**: (3, 3), (10, 10), (12, 12)
- **New Point**: (-5, 10)
- **Euclidean Distances**:
  - To (3, 3): 
    \[
    D = \sqrt{(-5 - 3)^2 + (10 - 3)^2} = \sqrt{64 + 49} = \sqrt{113} \approx 10.63
    \]
  - To (10, 10): 
    \[
    D = \sqrt{(-5 - 10)^2 + (10 - 10)^2} = \sqrt{225} = 15
    \]
  - To (12, 12): 
    \[
    D = \sqrt{(-5 - 12)^2 + (10 - 12)^2} = \sqrt{289 + 4} = \sqrt{293} \approx 17.1
    \]
- **Closest Cluster Mean**: (10, 10).

## 5. Hard K-Means Clustering Example
- **Points**: P(1,1), Q(2,1), R(4,3), S(5,4)
- **Initial Centroids**: C1 = (0, 0), C2 = (4, 4)
- **Iterations**:
  1. **First Assignment**: Assign points to the nearest centroid.
  2. **Update Centroids**: Calculate new cluster means.
  3. **Repeat** until convergence.
- **Final Centroids**: After convergence, new centroids are C1 = (1.5, 1) and C2 = (4.5, 3.5).

## 6. Kernel Function
- **Definition**: A kernel function computes the inner product of two vectors in a higher-dimensional space without explicit mapping.
- **Types of Kernels**:
  - **Linear Kernel**: 
    \[
    k(\mathbf{x}, \mathbf{y}) = \mathbf{x}^T \mathbf{y}
    \]
  - **Polynomial Kernel**: 
    \[
    k(\mathbf{x}, \mathbf{y}) = (\mathbf{x}^T \mathbf{y} + c)^d
    \]
  - **Radial Basis Function (RBF) Kernel**: 
    \[
    k(\mathbf{x}, \mathbf{y}) = \exp\left(-\frac{||\mathbf{x} - \mathbf{y}||^2}{2\sigma^2}\right)
    \]
  - **Sigmoid Kernel**: 
    \[
    k(\mathbf{x}, \mathbf{y}) = \tanh(\alpha \mathbf{x}^T \mathbf{y} + c)
    \]
- **Benefits**:
  - **Non-linearity**: Enables modeling of complex relationships.
  - **Efficiency**: Reduces computational costs with the kernel trick.
  - **Flexibility**: Different kernels can fit various data structures.

## 7. Transformation Mapping for Kernel
- **Given Kernel**: 
  \[
  k(x_1, y_1, x_2, y_2) = 1 + x_1y_1 + x_2y_2 + x_1y_1x_2y_2
  \]
- **Transformation Mapping**:
  \[
  \phi(x, y) = \begin{bmatrix} 1 \\ x \\ y \\ xy \end{bmatrix}
  \]
- **Dot Product Representation**: 
  \[
  k(\mathbf{x_1}, \mathbf{x_2}) = \phi(x_1, y_1)^T \phi(x_2, y_2)
  \]
