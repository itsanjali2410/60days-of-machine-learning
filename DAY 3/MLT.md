# 1.3 Representation Learning

## Overview
Representation learning is a subfield of unsupervised learning that focuses on extracting meaningful features or structures from data without any labeled responses. The primary goal is to learn a representation of the input data that captures its essential characteristics, making it easier for algorithms to process and analyze.

## Key Concepts

### Unsupervised Learning
Unsupervised learning techniques allow us to discover patterns in data without predefined labels. This process is crucial for extracting useful information from datasets that may not have explicit guidance.

### Compression and Comprehension
comprehension is nothing but compress the things you have learned. Explain something you have conprehentated, which means you have compressed the things to you.

Note: Using coefficient and representative we can reconstruct any dataset.

## Important Terms

### 1. Representative (\(n\))
- **Definition**: In the context of representation learning, a "representative" typically refers to the number of data points or samples in the dataset, denoted as \(n\).
- **Example**: If you have a dataset with 100 points, then \(n = 100\).
### 2. Coefficient (\(d\))
- **Definition**: The "coefficient" relates to the number of features or dimensions in the data, denoted as \(d\). Each data point can be represented as a \(d\)-dimensional vector.
- **Example**: In a dataset where each data point is described by three features (e.g., height, weight, and age), then \(d = 3\). The representation learning process focuses on transforming these \(d\) features into a more informative representation.

What is a proxy here?
As we know from our school days it refers to some known person taking the position on the permanent post for some sort of time. which means here when we have different points lined uo but one is odd man out not in the line so behalf of that point we take the projection of the point and project it on the line.

## Conclusion
if you had a bunch of data points, such that all of them lined up along the
line, then you can choose a representative and a coefficient for each of these data point.
But now we then said that, hey, only four points lie along the line, the first point
does not lie along the line, then we looked for a proxy on this line and we said that well,
you can just project this point onto this line, and then you are done. Which means that we need
to know where this point lies along this line. And that just is given by x transpose w, multiplied by
the vector w. That is nice, but it is still not completely does not complete our requirements.

1.4 Representation part 2

Goal: find a dataset which has least reconstruction error.

The reconstruction error is both +ve and -ve values.

The w is the eigrnvalues vector correspondint to the maximum eigenvalue vector.
