# Unsupervised Learning - Simplified Overview

Unsupervised learning is a type of machine learning where the goal is to understand and find patterns in a dataset that doesn't have labels or predefined outcomes. The data consists of **d-dimensional vectors**, and the task is to uncover hidden structures within this data.

### Major Tasks in Unsupervised Learning

1. **Dimensionality Reduction**: Reducing the number of features (dimensions) in the data while retaining important information.
2. **Clustering**: Grouping data points into similar categories.

## Dimensionality Reduction Simplified

The goal of **dimensionality reduction** is to compress the data while keeping important aspects and removing unnecessary details. This is useful when working with very high-dimensional data that is hard to analyze directly.

### Encoder and Decoder

- **Encoder (f)**: Compresses the original data (d-dimensional vector) into a lower-dimensional representation (d' < d).
- **Decoder (g)**: Reconstructs the original data from the compressed version. We aim for the reconstructed data `g(f(xi))` to be as close as possible to the original data `xi`.

### Loss Function

We use a **loss function** to measure how well the decoder works. It computes the difference between the original data `xi` and the reconstructed data `g(f(xi))`. The goal is to make this difference (loss) as small as possible.

\[
\text{Loss} = \frac{1}{n} \sum_{i=1}^{n} \left( g(f(x_i)) - x_i \right)^2
\]

This measures the average error over all data points.

### Real-life Example of Dimensionality Reduction

Suppose a production company receives 100,000 tweets about their latest release. Instead of showing all the tweets to the manager, you can use dimensionality reduction techniques to group them into 10 different types (or categories). Each category summarizes a different aspect of public opinion, making it easier to analyze the data.

---

By using **dimensionality reduction**, we simplify complex datasets while retaining the most important information.
